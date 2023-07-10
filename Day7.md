# Day7
## - Loops
In JavaScript, loops are used to repeatedly execute a block of code until a certain condition is met. There are several types of loops available in JavaScript.

- Noraml for loop
``` javascript
let Nums = [1 , 2 , 3 , 4 , 5];
for(let i = 0; i < Nums.length; i++){
  console.log(Nums[i]);
}
// 1 2 3 4 5;
```
- While (loop)
``` javascript
let i = 0;
while(i < 5){
console.log("HI");
}
// HI HI HI HI HI
```
- For of loop
``` javascript
cosnt city = ["Hebron" , "Gaza" , "Jerico"];
for(let ch of city){
console.log(ch);
}
// Hebron Gaza Jerico
```
## - Map

In JavaScript, the map() method is used to iterate over an array and transform each element into a new value. It creates a new array with the results of calling a provided function on every element in the original array, without modifying the original array. The map() method does not change the original array; instead, it returns a new array with the transformed values.
``` javascript
const numbers = [1, 2, 3, 4, 5];

const multipliedByTwo = numbers.map(function (num) {
  return num * 2;
});
// const multipliedBytwo = numbers.map(num => num * 2);
console.log(multipliedByTwo);
// Output: [2, 4, 6, 8, 10]
```
## - Filter
In JavaScript, the filter() method is used to create a new array that contains elements from the original array that pass a certain condition. It iterates over each element of the array and returns a new array with only the elements that satisfy the provided filtering function.
``` javascript
const numbers = [1, 2, 3, 4, 5];

const evenNumbers = numbers.filter(function (num) {
  return num % 2 === 0;
});
// const evenNumbers = numbers.filter(num => (num % 2) - 1); // numbers.filter(num => (num % 2) === 0);

console.log(evenNumbers);
```
## - Spread
In JavaScript, the spread syntax, denoted by three dots (...), is used to expand elements of an iterable (like an array or a string) or object properties into various contexts, such as function arguments, array literals, or object literals. It provides a concise way to manipulate and combine arrays, objects, and other iterable data structures.
- Array spread
``` javascript
const arr = [1, 2, 3];
const newArr = [...arr, 4, 5];
console.log(newArr);
// [1, 2, 3, 4, 5]
```
- objece spread
``` javascript
const obj1 = { a: 1, b: 2 };
const obj2 = { c: 3, d: 4 };
const mergedObj = { ...obj1, ...obj2 };
console.log(mergedObj);
// { a: 1, b: 2, c: 3, d: 4 }
```
- String Spread
``` javascript
const str = 'Hello';
const chars = [...str];
console.log(chars);
// ['H', 'e', 'l', 'l', 'o']
```
- setTimeout
In JavaScript, the setTimeout() function is used to schedule the execution of a function after a specified delay. It allows you to introduce a time delay in your code, making it useful for implementing timeouts, animations, or any scenario where you want to execute code after a certain period of time.
``` javascript
function sayHello() {
  console.log('Hello!');
}

setTimeout(sayHello, 2000);
// After 2 seconds, it will log "Hello!"
// 1000 equal to one second

function greet(name) {
  console.log(`Hello, ${name}!`);
}

setTimeout(greet, 2000, 'John');
// After 2 second greet function will output Hello John
```
```
