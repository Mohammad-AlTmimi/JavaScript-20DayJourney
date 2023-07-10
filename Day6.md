# Day 6
## - Attribute 
In JavaScript, an attribute refers to a characteristic or property of an HTML element that can be accessed and manipulated using JavaScript. Attributes are defined within the HTML tags and provide additional information about the elements.
- Disable Attribute
``` javascript
let button = document.getElementById("Button");
button.disable = true;
// In this situation the button is no longer able to click on it
```
## But how to set any Attribute in element
``` javascript
//element.setAttribute(attributeName, attributeValue);
//myElement.setAttribute('id', 'newDiv');
let button = document.getElementById("Button");
button.setAttribute("disable" , "") // button is no longer disable;
```

## There is a way to remove Attribute in JavaScript
``` javascript
//element.removeAttribute(attributeName);
let button = document.getElementById("Button");
button.removeAttribute("disable"); // button is no longe disable;
//button.removeAttribute("src"); // src is a class
``` 

## Scope

In JavaScript, the term "scope" refers to the visibility and accessibility of variables, functions, and objects within a particular part of your code. Scopes determine which variables are accessible in different parts of your code and how changes to those variables are propagated.
### JavaScript has three main types of scope:
- Global Scope: Variables declared outside any functions or blocks have global scope. They are accessible from anywhere in the code, including other functions and blocks.

- Function Scope: Variables declared within a function have function scope. They are only accessible within the function itself and any nested functions.

- Block Scope (Introduced in ECMAScript 6): Variables declared within blocks (e.g., within if statements or loops) have block scope. They are only accessible within the block where they are declared.
