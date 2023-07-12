# Day9
## - Function 
### - Higher order Function 

In JavaScript, higher-order functions are functions that can accept other functions as arguments and/or return functions as their results. They are a powerful feature of functional programming and enable you to write more concise and expressive code.
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
    
### - CallBack Function

