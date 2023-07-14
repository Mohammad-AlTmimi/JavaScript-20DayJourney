# Day10
## Closure in JavaScript

In JavaScript, closures are an important concept that refers to the ability of a function to access variables from its outer scope, even after the outer function has finished executing. In simpler terms, a closure is created when a function "remembers" its lexical scope and can access variables from that scope, even when the function is executed in a different scope.
## multiple clousure instance

In JavaScript, you can create multiple instances of closures by invoking the outer function multiple times. Each invocation will create a new closure with its own set of variables.
``` javascript
function createCounter() {
  var count = 0;

  function increment() {
    count++;
    console.log(count);
  }

  return increment;
}

var counter1 = createCounter();
var counter2 = createCounter();

counter1(); // Output: 1
counter1(); // Output: 2

counter2(); // Output: 1
counter2(); // Output: 2
```
## Practice
[Exercises for closures](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week2-day2-tasks/tasks.md)
- Question 1
``` javascript
function createCounter(start) {
  var counter = start;

  function increment() {
    counter++;
    return counter;
  }

  return increment;
}

// Example usage:
var counter = createCounter(5);

console.log(counter()); // Output: 6
console.log(counter()); // Output: 7
console.log(counter()); // Output: 8
```
- Question 2
``` javascript
function calculateAverage(nums) {
  var sum = nums.reduce((acc, num) => acc + num, 0);
  var count = nums.length;

  function average() {
    return sum / count;
  }

  return average;
}
var avg = calculateAverage([1, 2, 3, 4, 5]);
console.log(avg()); // Output: 3
```
- Question 3
``` javascript
function powerOf(base) {
  return function(exp) {
    return Math.pow(base, exp);
  };
}
var powerOfTwo = powerOf(2);
console.log(powerOfTwo(3)); // Output: 8

var powerOfThree = powerOf(3);
console.log(powerOfThree(4)); // Output: 81
```
- Question 4
``` javascript
function compose(...functions) {
  return function(input) {
    return functions.reduceRight((acc, func) => func(acc), input);
  };
}
function addOne(num) {
  return num + 1;
}

function double(num) {
  return num * 2;
}

function square(num) {
  return num * num;
}

var composedFunction = compose(square, double, addOne);
console.log(composedFunction(2)); // Output: 36
```


