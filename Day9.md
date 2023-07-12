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
