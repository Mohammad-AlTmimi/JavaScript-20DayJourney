# Day 14
## Practice
- ## Question One
``` javascript
for (var i = 0; i < 5; i++) {
    function a (index) {
      setTimeout(function() {
        console.log("value of [i] is: ", index);
      }, 100);
    };
    a(i);

  }
```
- ## Question Two
``` javascript
let array = [];
for (let i = 0; i < 5; i++) {
   array.push(i);
}

console.log("Current array is: ", array);
```
- ## Question Three
``` javascript

let functions = [];
for (var i = 0; i < 5; i++) {
    (function (index) {
        functions.push(() => {
            console.log("Current value of i is:", index);
            });
    } , (i))
}

functions.forEach((func) => func());
```
- ## Question Four
- ### Part one:
``` javascript
function privateCounter() {
  let count = 0;

  return {
    increment: function() {
      count++;
    },
    getCount: function() {
      return count;
    }
  };
}

let a = privateCounter();
a.increment();
console.log('a: ', a.getCount()); // Output: a: 1
a.increment();
console.log('a: ', a.getCount()); // Output: a: 2
```
- ### Part two:
``` javascript
