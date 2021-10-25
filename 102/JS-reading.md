# What is JavaScript?
JavaScript is a programming language that features first-class functions, that allows you to implement complicated features on a webpage. It is used in Node.js, Apache, and Adobe Acrobat which are non browser based environments. JavaScript should not be confused with Java. While both languages are trademarks of the company Oracle, they both use very different syntax, semantics, and are used for different reasons. 

## What is it used for?
In Web development, it is used as a scripting language that allows the developer to create dynamically updating content. JS can be used to store values within variables such as for a username request prompt. It can run a specific code in response to user input on the web page, such as changing the cursor when they hover their mouse over a link to show them it is clickable. 

## APIs
JavaScript includes built in functionality for Application Programming Interfaces (APIs). An API is essentially a conveniency shortcut, it provides the developer with a prebuilt section of code to produce a program. 

### Browser APIs
Prebuilt into your Internet Browser and enable you to perform a variety of useful complex things.
* The Document Object Model (DOM) allows you to control HTML and CSS, to be able to change the content and appearance of your webpage. 
* The Geolocation API enables geographical information, which is how Google Maps is able to tell you where you are on a map. 
* Audio and Video APIs allow you to play audio and video right in your webpage, similar to how YouTube works. 

### Third Party APIs
Do not come prebuilt into your Internet Browser, you have to manually find these through the Web. These can include a Twitter API which lets you post your twitter feed onto your website. 

## How to add JavaScript to your page
JavaScript can be added to your HTML page in a few different ways, Internally, Externally, and Inline. Similar to CSS however the difference is that with JS you only need one element. "Script"

### Internal JavaScript
The simplest way to add Internal Javascript to your code is to surround it with "script" tags. 

### External JavaScript
Create a file within the same directory as your HTML file, make sure your file name ends with a ".js"
You can place all of your JS code within your .js file, just make sure to connect your html file with a "script src="filename.js" defer" 

## Script Loading Strategies
JavaScript loads in the order in which it appears. This can be problematic at times because if you are using JS to manipulate a specific element that does not appear on your HTML until after where you've placed your script, then it won't work as intended. The old fashioned solution to this was to put all of your scripts at the body of your page, right before the closing body tag. The problem with this solution is that none of scripts will load until the browser has loaded all the HTML, and on larger sites this will lead to long load times due to the number of scripts they have to process at the end. 

### async and defer
Async loads the scripts while also allowing the html to be loaded. However your scripts will exectue as soon as they're loaded which can block the page rendering. Async is best used when all of your scripts run independently from each other and don't interact with each others elements. Scripts loaded with the defer attribute will load as they appear on the page, the difference is that it won't run the scripts until all of your content has loaded as well. 

## Comments
You can place comments by placing two forward slashes if it's a single line comment. If you have a multi line comment you can place it in between forward slashes with an asterisk. 
/* comment
goes
here
*/ for example. 

# Variables
There are 3 ways to declare a JavaScript variable: "var", "let", and "const". Variables are data values that have been stored. For example let price1 = 10. let price2 = 15. let total = price1 + price2. In this example we declared two separate variables, and used the third variable to calculate the final price of our product. 

## Identifiers
Variables have to be identified with specific names. Identifiers don't have to follow any naming conventions, they can be short and simple, or long and complex. However it's important to note that Identifiers are case sensitive, and must begin with a letter, a dollar sign, or an underscore.

## Assignment Operator
In JavaScript, the equal sign ( = ) is used as an assignment operator instead of an equal to operator. The equal to operator is a double equal sign( == ). 

## Data Types
The three main data types for this class are Strings, Numbers, and Booleans. Strings put simply are text, Numbers are self explanatory, and Booleans are True/ False statements.  

[BACK](https://github.com/Jrc2855/reading-notes/blob/main/README.md) 