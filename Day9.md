# Day9
## - Function 
### - Higher order Function 

In JavaScript, higher-order functions are functions that can accept other functions as arguments and/or return functions as their results. They are a powerful feature of functional programming and enable you to write more concise and expressive code.
``` javascript
function Hello(){
    console.log("Hello");
    function multibytwo(item){
        return item * 2;
    }
    return multibytwo;
}
cosnt HI = Hello(); // Hello
console.log(HI(2)) // 4
```
    
### - CallBack Function
In JavaScript, a callback function is a function that is passed as an argument to another function and is invoked or called at a later point in time. Callback functions are commonly used in asynchronous programming or to handle events.

``` javascript
function Operation(fac , arr){
    const newArr = arr.map(item = > fac(item));
    return newArr;
}
function multibytwo(item){
  return 2 * item;
}
  console.log(multibytwo , [1 , 2 , 3]) // Output = 2 4 6
```
### Way of writing function 

``` javascritp
function mulitby2(intput) {return input * 2} // 1
const multiby2 = (intput) =>{return input * 2} // 2
const multiby2 = (intput) => input * 2; // 3
const multiby2 = input => input * 2; // 4
```

## Practice
- [Use Higher-Order Functions map, filter, or reduce to Solve a Complex Problem](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-higher-order-functions-map-filter-or-reduce-to-solve-a-complex-problem)
``` javascript
const squareList = arr => {
  // Only change code below this line
  const newArr = [];
  arr.map(item => {
    if(item % 1 == 0 && item > 0)
      newArr.push(item * item);
      return ;
  })
  return newArr;
  // Only change code above this line
};

const squaredIntegers = squareList([-3, 4.8, 5, 3, -3.2]);
console.log(squaredIntegers);
```
- [Apply Functional Programming to Convert Strings to URL Slugs](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/apply-functional-programming-to-convert-strings-to-url-slugs)
``` javascript
// Only change code below this line
function urlSlug(title) {
  return (title.trim()).split(/\s+/)
.map(word => word.toLowerCase())
    .join("-");
}
// Only change code above this line
urlSlug("A Mind Needs Books Like A Sword Needs A Whetstone");
```
- [Exercises for functions and callbacks](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week2-day1-tasks/tasks.md)
``` javascript
function newAsync(value) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      if (value % 2 === 0) {
        resolve(value * 2);
      } else {
        reject(new Error("Error: Odd number encountered"));
      }
    }, 1000);
  });
}

const arr = [1, 2, 3, 4];

function mapAsync(arr) {
  const Newarr = arr.map(item => {
    return newAsync(item).catch(error => {
      return error.message;
    });
  });
  return Newarr;
}
```
[Call Stack and Recursion](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week2-day1-tasks/tasks.md)
``` javascript
function sumRange(start, end) {
  if (start === end) {
    return start;
  } else {
    return start + sumRange(start + 1, end);
  }
}
```
