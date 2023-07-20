# Day13
## TypeScript
TypeScript! TypeScript is a superset of JavaScript that adds static typing to the language, making it easier to catch errors and write more robust code. Here's a basic introduction to TypeScript:
## Type in TypeScript
``` typescript
// Variable with type 
let message: string = "Hello, TypeScript!";

// Function with type annotations
function add(a: number, b: number): number {
  return a + b;
}

// Calling the function
let result: number = add(5, 10);

console.log(message);
console.log("The result of the addition is:", result);
```
## Practice
[TypeScript](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week3-day3-tasks/tasks.md)
- Question one:
``` javascript
var one = 1;
const arrowHOF = (normalFunc) => {
    return (...args) => {
      return (count) => {
        if(!count)
            count = 1;
        const results = [];
        for (let i = 0; i < count; i++) {
          results.push(normalFunc(...args));
        }
        return results;
      };
    };
  };
const exampleNormalFunc1 = (a, b, c) => {
  return a * (b + c);
}

const exampleNormalFunc2 = (x, y) => {
  return x * y;
}

const exampleNormalFunc3 = (string) => {
  return string + " " + string + " " + string + "!";
}
const hofNormalFunc1 = arrowHOF(exampleNormalFunc1);
const hofNormalFunc2 = arrowHOF(exampleNormalFunc2);
const hofNormalFunc3 = arrowHOF(exampleNormalFunc3);
console.log("hi")
 console.log(hofNormalFunc1(3, 4, 5)(2)); // logs 60 twice
 console.log(hofNormalFunc2(20, 35)(4)); // logs 700 four times
 console.log(hofNormalFunc3("Meow")());
```

