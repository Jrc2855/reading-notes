# Chapter 3: Object Literals

## What is an Object?
An object groups together a set of variables and functions to create a model of something you would recognize from the ral world. In an object, variables and functions take on new names. 

* When variables are in an Object, they are now considered properties. 
* When functions are in an Object, they are considered methods. 

Like variables and named functions, properties(variables) and methods(functions) have a name and a value. In an object, that name is called a **key**. The reason it's called a key is because it is keys are used to access their corresponding value.

## Example Object

```js
let hotel = { // 'hotel' is the name of this object.
  name: 'Quay', //Each of these Variables are now considered Properties because they are inside of an Object.
  rooms: 40,
  booked: 25,
  checkAvailability: function(){ //This function is now considered a Method because it is inside of an Object. 
    return this.rooms - this.booked; //'this'returns a Property or function from the Object they are inside of.
  }
}
```

## Creating an Object: Literal Notation
The easiest and most popular way to create objects. The object is the curly braces and their contents. 
Declare a variable using "let" (they used to declare this variable with var, but then JS added "let" which is much more Function scoped.) followed by an assignment operator and a curly bracket. All of your properties come after the curly bracket.

## Accessing an object and DOT notation
You access the properties or methods of an object using dot notation. You can also access properties using square brackets. To access a property or method of an object you use the name of the object, followed by a period. then the name of the property or method you want to access. For example following our 'hotel' Object above.

```js
let hotelName = hotel.name; // 'hotel' is the object name, the period is the member operator, and the property is called afterwards.
let roomsFree = hotel.checkAvailability();
```

You can also access properties using square brackets. 
```js
let hotelName = hotel['name'];
let roomsFree = hotel['checkAvailability']()
```

To access a property of this object, the object name is followed by a dot (the period symbol) and the name of the property that you want. Similarly, to use the method, you can use the object name followed by the method name. 

```js
//Going off our example above.
let elName = document.getElementById('hotelName');
elName.textContent = hotel.name;

let elRooms = document.getElementById('rooms');
elRooms.textContent = hotel.availability();
// These examples show how to access properties of our Object.
```



# Chapter 5: Document Object Model
As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes. Every element, attribute, and piece of text in the HTML is represented by its own DOM node.

## Document Node
At the top of the DOM tree the document node is added; it represents the entire page. When you access any element, attribute, or text node, you navigate to it via the document node. It is the starting point for all visits to the DOM tree. Think of it like the trunk of the DOM tree.

## Element Nodes
HTML elements describe the structure of an HTML page. (<H1> - <H6>, <p>, etc...)To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to. Relationships between the document and all of the element nodes are described using the same terms as a family tree: parents, children, siblings, ancestors, and descendants. (Every node is a descendant of the document node.)

## Attribute Nodes
The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree. Attribute nodes are not children of the element that carries them; they are part of that element. Once you access an element there are specific JavaScript methods and properties to read or change that element's attributes. 

## Text Nodes
Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node. Text nodees cannot have children. If an element contains text and another child element, the child element is not a child of the text node but rather a child of the containing element. This illustrates how the text node is always a new branch of the DOM tree, and no further branches come off of it. 

## Working with the DOM tree
Accessing and updating the DOM tree involves two steps: 
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.

## Step 1: Access the Elements

### Selecting individual elements
Here are three common ways to select an individual element:
'getElementById()' Uses the value of an element's id attribute
'querySelector()' Uses a CSS selector, and returns the first matching element.
You can also select individual elements by traversing from one element to another within the DOM tree

### Selecting Multiple Elements
There are three common ways to select multiple elements:
'getElementsByClassName()' Selects all elements that hae a specific value for their class attribute
'getElementsByTagName()' Selects all elements that have the specified tag name.
'querySelectorAll()' Uses a CSS selector to select all matching elements.

### Traversing Between Element Nodes
You can move from one element node to a related element node.
'parentNode' Selects the parent of the current element.
'previousSibling / nextSibling' selects the previous or next sibling from the DOM tree.
'firstChild / lastChild' selects the first or last child of the current element.

## Step 2: Work with those Elements

### Access/ Update Text Nodes
The text inside any element is stored inside a text node. To access the text node. 1) Select the <li> element 2) Use the firstChild property to get the text node 3) Use the text node's only property (nodeValue) to get the text from the Element. nodeValue - This property lets you access or update contents of a text node. 

### Work with HTML Content
One property allows access to child elements and text content: 'innerHTML' 
Another just the text content: 'textContent'
Several methods let you create new nodes, add nodes to a tree and remove nodes from a tree: 'createElement()', 'createTextNode()', 'appendChild() / removeChild()' This is called DOM manipulation

### Access or Update Attribute Values
Here are some of the properties and methods you can use to work with attributes: 'className/ id' Lets you get or update the value of the class or id attributes. 
'hasAttribute()' Checks if an attribute exists.
'getAttribute()' Checks the Value of an attribute.
'setAttribute()' Updates the value of an attribute.
'removeAttribute()' Removes an attribute