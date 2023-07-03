# Day 1: Basic instruction in JavaScript
## 1.What is JavaScript 
JavaScript is a versatile and popular programming language used primarily for web development. It is often referred to as the "language of the web" because it runs on web browsers and enables interactivity and dynamic functionality on websites.

JavaScript was created in 1995 by Brendan Eich and initially designed to provide basic scripting capabilities within web browsers. However, it has since evolved into a powerful language capable of performing a wide range of tasks beyond web development, including server-side scripting, desktop application development, game development, and more.

## 2.The Document Object Model (DOM)
The DOM in HTML is a programming interface that represents the structure of a web page as a hierarchical tree. It allows developers to access and manipulate HTML elements using JavaScript, enabling dynamic changes to content, style, and behavior. With the DOM, developers can create interactive web pages that respond to user actions.
// We can Represent DOM as Tree

## 3.document

In JavaScript, the term "document" refers to the Document Object Model (DOM) interface. The "document" object represents the web page loaded in the browser and provides methods and properties for interacting with and manipulating the HTML elements and content of the page.

```
var element1 = document.getElementById("myElement");
//This code retrieves the element with the ID "myElement" and assigns it to the variable element1.

var element2 = document.querySelector(".myClass");
//This code selects the first element with the class "myClass" and assigns it to the variable element2.

var elements3 = document.querySelectorAll(".myClass");
//This code selects all elements with the class "myClass" and assigns them to the variable elements. The result is a NodeList, which is a collection of elements //that you can iterate over or perform operations on.
```
