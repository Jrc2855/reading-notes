# CSS
CSS aka: Cascading Style Sheets allow you to control the appearance of your web page. 
By default the browser will style everything according to an built in stylesheet. This is to ensure that headings are properly formatted, links are highlighted, and lists and tables appear the way you initially designed them to look. 
CSS can be used for customizing the size and color of text on your page, or creating a layout such as a column of hyperlinks to the left of your main content area. It can even be used for adding effects to your site, such as animating images. 

## Syntax
CSS is known as a rule based language, which means it will follow the rules that you designate for particular elements, or groups of elements. For example if you want all of your H1 headers to be bright red. 

### Selectors 
The selector is the HTML element that you are applying your CSS to. You then use a set of Curly braces to create declarations which are changes to the properties you would like to customize, and the values you want them to have. 

### Modules 
CSS as a language is broken down into modules. This can make it easier to find specific types of CSS language such as Backgrounds and Borders, or Font, etc...

## Inserting a style sheet
Their are three main ways of inserting a style sheet into your HTML pages. 

### External CSS
Within your HTML page you must include a link to the external style inside your HEAD element. 
It can be written by any text editor as long as it has a .css extension at the end of the file name.
Can not contain any HTML tags.

### Internal CSS 
Can be used if one single page on your site needs a specific style. 
To implement an Internal sheet, you need to put a style tag in your HTML file, specifically in the head section. 

### Inline CSS
Can be used to apply a specific style to a single element. 
When you place your opening tag for your HTML element, add "style" to it and simply type your CSS into the opening tag. 

## Multiple style sheets
If you have several style sheets for the same selector (element) then only the style sheet that is read last will be used. 

## Cascading Order
If multiple methods are used to style an element it will follow the following order: Inline Style, External and Internal style sheets, and it will use the Browser default last. 


[BACK](https://github.com/Jrc2855/reading-notes/blob/main/README.md) 


