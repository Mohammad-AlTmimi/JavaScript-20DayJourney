# Day4

## Sort
The sort() function in JavaScript treats the elements of an array, including strings, and sorts them in alphabetical order.
for example 
``` javascript
let arr = [10 , 20 , 5 , 8].sort()  // we Expected to be [5 , 8 , 10 , 20]
                                    // But in JavaScript it will be [10 , 20 , 5 , 8]
```

## join
We can use join in array to join element to the array 
for example 
``` javascript
let arr = ["Mohammad" , "Tamimi" , "Friend"];
arr.join("&");
console.log(arr) // Mohammad&Tamimi&Friend
```

## mutable vs immutable
in JavaScript there is mutable data and immutable data
### - muttable data 
like array (we can change the data in side it)
``` javascript
let arr = ["Mohammad" , "Ali"];
arr[1] = "Tamimi";
console.log(arr) // Mohammad Tamimi
```
### - immutable data
like string and primitives
``` javascript
let s = "Mohammaa";
s[7] = "d";
console.log(s) // Mohammaa;
// Note that (s[7] = "d" doesnot show compilation error but it did not work)
``` 

