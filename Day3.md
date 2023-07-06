# Day3

## variable in JavaScript

### - var 
Var is a way to declare a variable in JavaScript and it was the first method introduced in the language.
```
var car; // Undefined
car = "AUDI" // "AUDI"
```
### - let

In JavaScript, let is a keyword used to declare variables with block scope. Variables declared with let are only accessible within the block of code where they are defined, such as inside a function or an if statement.
``` javascript
let car; // Undefined
car = "AUDI" // "AUDI"
```
### So What the different between let and var

## - Scope:

Variables declared with var have function scope or global scope, depending on where they are declared. They are accessible throughout the function or global scope, even if declared inside a block.
Variables declared with let have block scope. They are only accessible within the block in which they are declared.
## - Hoisting:

Variables declared with var are hoisted to the top of their scope during the compilation phase, allowing them to be accessed before their declaration. However, the assignment remains in its original place.
Variables declared with let are also hoisted to the top of their scope, but unlike var, they are not initialized. They enter a "temporal dead zone" and cannot be accessed before their declaration.

## Note: 
- There's a different between assign a value and declare a value in JavaScript
```
let x; // declare
x = 10; // assign
```
- In JavaScript you can chagne the type of the variable in JavaScript
```
let x = 10; // x = 10
x = "Mohammad" // x = "Mohammad"
```
## - Array
Like other language JavaScript also had a Array
index in array start from zero (0)
```
let x = []; // intialize an array
```

## Practice:
- [Return a Value from a Function with Return](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/global-scope-and-functions)
- [Global Scope and Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/global-scope-and-functions)
- [Local Scope and Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/local-scope-and-functions)
- [Global vs. Local Scope in Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/local-scope-and-functions)
- [Stand in Line](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/global-vs--local-scope-in-functions)
