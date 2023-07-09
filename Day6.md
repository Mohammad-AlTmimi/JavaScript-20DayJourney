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
