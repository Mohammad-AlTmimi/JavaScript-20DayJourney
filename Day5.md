# Day5

## Function 
A function in JavaScript is a reusable block of code that performs a specific task or calculates a value. It is a fundamental building block of JavaScript programming and allows you to organize and encapsulate logic into reusable units.

A JavaScript function can be defined using the function keyword followed by the function name, a set of parentheses (), and a block of code enclosed in curly braces {}. 
``` javascript
function sum(num1 , num2){
  return num1 + num2;
}

```
We can also write variable hold function 
``` javascript
const sum = (num1 , num2) =>{
  return num1 + num2;
}
// This code work exactly the same from the first one
```
- # practice
``` javascript
async function fetchData() {
try {
    const response1 = await fetch('https://rickandmortyapi.com/api/character');
    const response2 = await response1.json();
    let filer = response2.results.filter(item => item.status === 'Alive')
    if(filer.length > 50){
        const filer = filer.splice(0 , 50);
    }
    console.log(filer)
  } catch (error) {
    console.error('Error fetching data:', error);
  }
}
fetchData();
```
