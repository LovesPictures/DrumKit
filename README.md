
##
# Project 1: JavaScript Drum Kit

Judith Ricketts, Artist, Lecturer and Software Engineer - [Contact](https://lovespictures.com/)  
Commit Date: 25th October 2021

An HTML page displays a collection of `div` elements, each containing a letter
  that corresponds with a key on the keyboard, and the name of the soundclip to be
  played when that button is clicked. When a user presses a key that matches
  one of the letters displayed in the `div` elements, the page should play 
  the corresponding soundclip and place a temporary 'highlight' (or border) 
  around the `div`. Write the JavaScript code necessary to add this functionality.

## Guide

The HTML, CSS, and sound clips were provided as starter code.

- HTML `data-*` attributes: Introduced in HTML5, `data-*` attributes (where * can
    be anything) allows us to store _custom data_ on any HTML element. Each
    `div.key` (`<div class="key" data-key="...">`) and `audio` element in the 
    provided HTML file has a `data-key` attribute which corresponds with a keyboard button.

- CSS `playing` class & pre-defined style: The CSS file provided has a `playing`
    class defined with some attributes.

- We use the `data-key` attributes to match the correct audio clip with the div element,
  and we can use the `playing` class to add that temporary highlight/border.


## Useful links
 
* [Add Sound to your JavaScript game with Howler JS (not VanillaJS!)](https://www.youtube.com/watch?v=hn7MhPt24L4&ab_channel=DrewConley)
* [Sound board with vanilla JavaScript](https://www.youtube.com/watch?v=E-v4SSCG6i4&ab_channel=WebDev)



<!-- **Steps:**

 1. Add an _event listener_ to the entire window object that is listening for a 
  `keydown` event; the function that we will provide as the _callback_ will be
  defined next. For now, decide on what the function name will be and provide
  that name as the second argument for our event listener.

2. Create a function with the name that you decided on in step 1. 
    - The function should accept one parameter, the _event_ which the function is going to handle. 
    - In the body of the function, declare and define two variables that will 
      reference the  _div and audio elements_ that correspond with the keypress which 
      triggered the function (if such elements exist). 
    - If the key pressed doesn't match one of the keys defined on our page we don't 
      need to proceed any further, but if it does then we can use the variable 
      referencing the `div` element to add the `playing` class to it, and we can use 
      the variable referencing the `audio` element to play the audio file.

3. Declare & define a variable which will reference all the HTML elements on our
  page with a class `key`.

4. Iterate through the HTML elements and add an _event listener_ to each one that will
  fire on the `transitionend` event. Provide another function (name of your choice)
  as the second argument which will be responsible for **removing** the `playing`
  class.

5. Create a function with the name that was used in step 4.
    - This function (event handler) will fire when the `playing` class is added
      to an element and the transition animation completes. The event provided
      to the function as an argument will contain a reference to the `TransitionEvent`
      (or events) with the CSS property's name which was transitioned into.
    - The function should only be concerned with the `transform` property, as this
      property defines the time the animation will take, and we don't want to remove
      the class until the transformation is complete.
    - If there is an event with a property name `transform`, target the _function 
      context_ (the HTML element to which the event listener was attached) and remove
      the `playing` class.

 -->
