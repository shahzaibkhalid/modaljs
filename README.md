<p align="center">
  <a href="https://shahzaibkhalid.github.io/modaljs">
    <img alt="modal.js" src="https://raw.githubusercontent.com/shahzaibkhalid/modaljs/master/images/modaljs.png" width="400"/>
  </a>
  <h1 align="center">modal.js</h1>
</p>

<p align="center">
Chose from wide variety of iconic animations and build any kind of
notification popups, off-the-screen forms, beautiful nav bars and much
more!
</p>

## Use

You can create your interactive modal online and download it on the fly. Visit [modal.js website.](https://shahzaibkhalid.github.io/modaljs)

## Documentation

### How to download modal.js:

1.  Chose your input animation from drop down.
2.  Chose your output animation from drop down.
3.  Add/modify the HTML that you want to render inside the modal window.
4.  Add/modify the CSS to modify the modal window styling and the
    content inside the modal.
5.  Test how your modal will look like in your application using modal.js
    powerful online WYSIWYG editor.
6.  Download modal.js source file when you're satisfied with the look
    and content of modal window.

### How to use modal.js in your app

-   After you've downloaded `modal.js` file, include this JavaScript
    file at the bottom of HTML content, as shown below.

<!-- -->

      <body>
        ...
        <h1>I love modal.js</h1>
        ...
      </body>
      <script src="./modal.js"></script>
      

-   Then, you've to call the `openModal()` function to open the modal
    window.
-   There can be various ways to trigger `openModal()` function, let's
    trigger it using a button.

<!-- -->

      <body>
        ...
        <button> onclick="openModal()">Click to open modal</button>
        <h1>I love modal.js</h1>
        ...
      </body>
      <script src="./modal.js"></script>
      

That's it! Your modal window should work like a breeze now.

### How to modify modal.js HTML and animations after downloading

Now, theres an interesting but common case, you've downloaded the
`modal.js` file, but after downloading the file, you've found to modify
either the HTML being rendered inside the modal or the style of modal
itself.

-   Open `modal.js` file that you've downloaded.
-   Search for `document.body.innerHTML` in `modal.js file.`
-   You'll come along with following code snippet:

<!-- -->

      ...
      //HTML inside the modal and Input CSS animation tag
      document.body.innerHTML += 
        `<div class="modal" id="myModal">
          <div class="modal-content-area animated shake">
            <i class="close-button" aria-hidden="true">✖</i>
            
              <h1>Hello world</h1>
              <p>It's shahzaib here.</p>
              <p>Download resume</p>
            
            
          </div>
        </div>`;
      //Output CSS animation name              
      classesToHide = ['modal-content-area', 'animated', 'wobble'];
      //Input CSS animation tag
      classesToRetainOriginal = ['modal-content-area', 'animated', 'shake'];
      ...
      

-   Modal HTML code and both, input, output animation tags are
    highlighted in above code.
-   `shake` is input animation, while `wobble` is output animation.
-   You can make these changes in `modal.js` file to change animations
    and HTML content of modal window.

### How to modify modal.js styling after downloading

Now, after HTML content and animations, next thing to modify is CSS
styling of modal window and the HTML content within modal window.

-   Open `modal.js` file.
-   Search for `$modalCSS` first occurance in file.
-   Here's how the code looks like:

<!-- -->

      ...
      $outputAnimation: 'wobble',
      $modalCSS: `.modal {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.4);
        overflow:auto;
      }
      ...
      

That's it. Now, you can add or remove CSS style tags here and thus
modify modal window styling.

### What if I want to add more than one modal window on same page?

That's complicated! But there's a workaround.

-   Finalize your 2nd modal and download `modal.js` file.
-   Now go into file and find and replace all JavaScript variables,
    function names, e.g. replace `openModal()` with something like
    `openModalSecond()`.
-   Replace Style classes of only modal related CSS, e.g. replace
    `.modal` with `.modalSecond`.
-   Through this way, you can add as many distinct modal windows as you
    want and trigger them using their respective triggering functions.

## Inconsistencies?

If you find any inconsistency in any language, raise an Issue and I'll fix it.

## Developer

modal.js is written by [Shahzaib Khalid](shahzaibkhalid.com)

## License

modal.js is licensed under the MIT License.

Copyright (c) 2017 Shahzaib Khalid
