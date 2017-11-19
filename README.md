![modaljs](./images/modaljs.svg)

The most easiest way to add and modify interactive modal windows to a JavaScript applications. {.main-tagline}
----------------------------------------------------------------------------------------------

Chose from wide variety of iconic animations and build any kind of
notification popups, off-the-screen forms, beautiful nav bars and much
more!

Download Library

Read Docs

### Download Section {#download .section-heading}

#### How to download modal.js: {.sub-section-heading}

1.  Chose your input animation from drop down.
2.  Chose your output animation from drop down.
3.  Add/modify the HTML that you want to render inside the modal window.
4.  Add/modify the CSS to modify the modal window styling and the
    content inside the modal.
5.  Test how your modal will look like in your application using this
    powerful onlien WYSIWYG editor.
6.  Download modal.js source file when you're satisfied with the look
    and content of modal window.

Input Animation: bounce flash pulse rubberBand shake swing tada wobble
jello bounceIn bounceInDown bounceInLeft bounceInRight bounceInUp
bounceOut bounceOutDown bounceOutLeft bounceOutRight bounceOutUp fadeIn
fadeInDown fadeInDownBig fadeInLeft fadeInLeftBig fadeInRight
fadeInRightBig fadeInUp fadeInUpBig fadeOut fadeOutDown fadeOutDownBig
fadeOutLeft fadeOutLeftBig fadeOutRight fadeOutRightBig fadeOutUp
fadeOutUpBig flip flipInX flipInY flipOutX flipOutY lightSpeedIn
lightSpeedOut rotateIn rotateInDownLeft rotateInDownRight rotateInUpLeft
rotateInUpRight rotateOut rotateOutDownLeft rotateOutDownRight
rotateOutUpLeft rotateOutUpRight slideInUp slideInDown slideInLeft
slideInRight slideOutUp slideOutDown slideOutLeft slideOutRight zoomIn
zoomInDown zoomInLeft zoomInRight zoomInUp zoomOut zoomOutDown
zoomOutLeft zoomOutRight zoomOutUp hinge jackInTheBox rollIn rollOut \
 Output Animation: bounce flash pulse rubberBand shake swing tada wobble
jello bounceIn bounceInDown bounceInLeft bounceInRight bounceInUp
bounceOut bounceOutDown bounceOutLeft bounceOutRight bounceOutUp fadeIn
fadeInDown fadeInDownBig fadeInLeft fadeInLeftBig fadeInRight
fadeInRightBig fadeInUp fadeInUpBig fadeOut fadeOutDown fadeOutDownBig
fadeOutLeft fadeOutLeftBig fadeOutRight fadeOutRightBig fadeOutUp
fadeOutUpBig flip flipInX flipInY flipOutX flipOutY lightSpeedIn
lightSpeedOut rotateIn rotateInDownLeft rotateInDownRight rotateInUpLeft
rotateInUpRight rotateOut rotateOutDownLeft rotateOutDownRight
rotateOutUpLeft rotateOutUpRight slideInUp slideInDown slideInLeft
slideInRight slideOutUp slideOutDown slideOutLeft slideOutRight zoomIn
zoomInDown zoomInLeft zoomInRight zoomInUp zoomOut zoomOutDown
zoomOutLeft zoomOutRight zoomOutUp hinge jackInTheBox rollIn rollOut

#### HTML for Modal {style="text-align:center"}

#### CSS for Modal {style="text-align:center"}

Test Output

Download File

### Documentation {#documentation .section-heading}

#### How to use modal.js in your app {.sub-section-heading}

-   After you've downloaded `modal.js` file, include this JavaScript
    file at the bottom of HTML content, as shown below.

<!-- -->

      &ltbody>
        ...
        &lth1&gtI love modal.js</h1>
        ...
      </body>
      &ltscript src="./modal.js"></script>
      

-   Then, you've to call the `openModal()` function to open the modal
    window.
-   There can be various ways to trigger `openModal()` function, let's
    trigger it using a button.

<!-- -->

      &ltbody>
        ...
        &ltbutton> onclick="openModal()"&gtClick to open modal</button>
        &lth1&gtI love modal.js</h1>
        ...
      </body>
      &ltscript src="./modal.js"></script>
      

That's it! Your modal window should work like a breeze now.

#### How to modify modal.js HTML and animations after downloading {.sub-section-heading}

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
        `&ltdiv class="modal" id="myModal">
          &ltdiv class="modal-content-area animated shake">
            &lti class="close-button" aria-hidden="true">✖</i>
            
              &lth1&gtHello world</h1>
              &ltp&gtIt's shahzaib here.</p>
              &ltp&gtDownload resume</p>
            
            
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

#### How to modify modal.js styling after downloading {.sub-section-heading}

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

#### What if I want to add more than one modal window on same page? {.sub-section-heading}

That's complicated! But there's a workaround.

-   Finalize your 2nd modal and download `modal.js` file.
-   Now go into file and find and replace all JavaScript variables,
    function names, e.g. replace `openModal()` with something like
    `openModalSecond()`.
-   Replace Style classes of only modal related CSS, e.g. replace
    `.modal` with `.modalSecond`.
-   Through this way, you can add as many distinct modal windows as you
    want and trigger them using their respective triggering functions.

### Developer {.section-heading}

modal.js is written by [Shahzaib Khalid](shahzaibkhalid.com)

modal.js is being maintained on
[GitHub](https://github.com/shahzaibkhalid/modaljs)

### License {.section-heading}

modal.js is licensed under the MIT License.

Copyright (c) 2017 Shahzaib Khalid
