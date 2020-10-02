# JavaScript Drum Kit
Abdelrahman Hamdy , Senior Front-End Developer - [Contact](https://www.linkedin.com/in/abdeltahmanhmdy/)  
Last Commit Date: Oct 3, 2020

An HTML page displays a collection of `div` elements, each containing a letter
  that corresponds with a key on the keyboard, and the name of the soundclip to be
  played when that button is clicked. When a user presses a key that matches
  one of the letters displayed in the `div` elements, the page should play 
  the corresponding soundclip and place a temporary 'highlight' (or border) 
  around the `div`. Write the JavaScript code necessary to add this functionality.

## Guide

We are provided with the HTML, CSS, and sound clips necessary to create this
  page/application. Let's go over the provided files and look at the pieces
  that we can utilize to fulfill the requirements:

- HTML `data-*` attributes: Introduced in HTML5, `data-*` attributes (where * can
    be anything you want) allow us to store _custom data_ on any HTML element. Each
    `div.key` (`<div class="key" data-key="...">`) and `audio` element in the 
    provided HTML file has a `data-key` attribute which corresponds with a keyboard button.

- CSS `playing` class & pre-defined style: The provided CSS file already has a `playing`
    class defined with some rules in it. We will apply this class to the correct
    element, depending on the key pressed by the user, and remove it once animation
    is finished.

And that's...pretty much all we should need from the HTML & CSS files. We can use
  the `data-key` attributes to match up the correct audio clip with the div element,
  and we can use the `playing` class to add that temporary highlight/border.