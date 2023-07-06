# Day4

## Sort
The sort() function in JavaScript treats the elements of an array, including strings, and sorts them in alphabetical order.
for example 
``` javascript
let arr = [10 , 20 , 5 , 8].sort()  // we Expected to be [5 , 8 , 10 , 20]
                                    // But in JavaScript it will be [10 , 20 , 5 , 8]
```

## - join
We can use join in array to join element to the array 
for example 
``` javascript
let arr = ["Mohammad" , "Tamimi" , "Friend"];
arr.join("&");
console.log(arr) // Mohammad&Tamimi&Friend
```

## - mutable vs immutable
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
## - let vs const 
let and const have so many thing in common but there is one thing they have differnt in it
let variable can change it data unlike const 
``` javascript
let car = "AUDI"
car = 10; // No problem
const car = "AUDI"
car = 10; // compailation error
```
## - Object
An object is a data structure that encapsulates related data and functions into a single unit. It allows us to organize and manage information by grouping it together. Objects are used in programming to represent real-world entities or abstract concepts, and they enable us to write modular and reusable code.
``` javascript
let obj = {
  name: "Mohammd",
  age: 20,
  Universty: "Hebron Universty"
}
```
and there is also Nested Object
A nested object refers to an object that is nested or contained within another object. In other words, it is an object that is a property or value of another object. This nesting can occur at multiple levels, creating a hierarchical structure.
``` javascript
let person = {
  name: "John",
  age: 30,
  address: {
    street: "123 Main St",
    city: "New York",
    country: "USA"
  }
};
```
## - Practice 
[Use Multiple Conditional (Ternary) Operators](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-multiple-conditional-ternary-operators)
``` javascritp
function checkSign(num) {
    return (num === 0)? "zero": (num > 0)? "positive": "negative"
}

checkSign(10);
```
[Gold Code](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/golf-code)
``` javascript
const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
  // Only change code below this line
  let s;
  if(strokes === 1)
    s = "Hole-in-one!";
  else if(strokes  <= par - 2)
    s = "Eagle";
  else if(strokes === par - 1)
    s = "Birdie";
  else if(strokes === par)
    s = "Par";
  else if(strokes === par + 1)
    s = "Bogey";
  else if(strokes === par + 2)
    s = "Double Bogey";
  else if(strokes >= par + 3)
    s = "Go Home!"

  return s;
  // Only change code above this line
}

golfScore(5, 4);
```
[Use the map Method to Extract Data from an Array](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-map-method-to-extract-data-from-an-array)
``` javascript
const ratings = watchList.map(user => {
  return { title: user["Title"], rating: user["imdbRating"] };
});
```
[Use the filter Method to Extract Data from an Array](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-filter-method-to-extract-data-from-an-array)
``` javascript
const filteredList = watchList
  .filter(movie => parseFloat(movie.imdbRating) >= 8.0)
  .map(movie => ({ title: movie.Title, rating: movie.imdbRating }));

```




