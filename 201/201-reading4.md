# HTML Links, CSS Layout, JS Functions

## HTML Links

Links are one of the most significant features of the web, because they allow the user to change from one web page to another. Links are created using the HTML element '<a href='www.webpage.com'></a>' When linking to an external site it's important to use the full url which includes the 'http://'. To link to an Internal site you can use a relative url which looks like 'href='webpage.html'. 

## CSS Layout

CSS treats each HTML elements as if its in its own box. These boxes are typically considered one of two types. Block-level which means they start on a new line, and Inline which flow in between surrounding text. To control the positioning of each of these Elements there are several CSS Keywords that can be used.

* Normal Flow is the default behavior for Element Positioning and follows the rules of the type of element. Block-level elements start on a new line, and Inline flows in between the surrounding text.
* Relative Positioning shifts the element to the top, left, right, or bottom of where it normally would have rendered.
* Absolute Positioning completely removes the element from its previous position and places it depending on where the containing element is held. When the user scrolls, these elements move display, similar to an overlay.
* Fixed Positioning is a form of absolute positioning but does not move with the user scrolls.
* Floating Elements takes the element out of normal flow and position it to the far left or right of a containing box.

## JS Functions

Functions allow the developer to create a block of code that is designed to perform a singular specific task. This is excellent for reusability because the function can be called or invoked numerous times. Functions can take parameters which is information that is provided through various means, and return a specific value. When Variables are declared inside of a function they are considered Local Variables, and can only be used within that specific Function. If a variable is declared outside of a Function, it is considered a Global Function, and can then be called within multiple functions.