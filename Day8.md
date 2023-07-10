# Day8
## - API
In JavaScript, an API (Application Programming Interface) is a set of rules and protocols that allows different software applications to communicate and interact with each other. APIs enable developers to access and use the functionality of external services, libraries, or frameworks in their own applications.
## - Fetch

In JavaScript, the fetch() function is used to make HTTP requests to retrieve resources (data) from a server. It provides a modern and flexible way to handle asynchronous network requests. The fetch() function returns a Promise that resolves to the Response object representing the response to the request.
## - API and Fetch
``` javascript

function MohammadTamimi(car) {
  const url = `https://mohammadtamimi.com`;

  fetch(url)
    .then(response => {
      if (!response.ok) {
        throw new Error('Network response was not ok');
        // There is a problem with fetching api
      }
      return response.json();
    })
    .then(data => {
      console.log(`Mohammad Tamimi ${data}`);
    })
    .catch(error => {
      console.error('Error:', error);
      // It will type the error if its happen
    });
}

MohammadTamimi('AUDI');
```
## - await with Promises
In JavaScript, you can use the await keyword with Promises to write asynchronous code in a more synchronous and readable manner. The await keyword can only be used inside an async function, which is a function that returns a Promise.
``` javascript
function delay(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

async function run() {
  console.log('Start');

  await delay(2000);
  console.log('After 2 seconds');

  await delay(1000);
  console.log('After 1 more second');

  console.log('End');
}

run();
```
## - Array Destructuring

In JavaScript, destructuring assignment allows you to extract individual elements or properties from arrays and objects and assign them to variables in a concise way. It provides a convenient syntax for extracting values without explicitly accessing them by index or property name.

``` javascript
const numbers = [1, 2, 3, 4, 5];

// Extract individual elements
const [a, b, c] = numbers;
console.log(a); // Output: 1
console.log(b); // Output: 2
console.log(c); // Output: 3

// Ignore specific elements
const [x, , z] = numbers;
console.log(x); // Output: 1
console.log(z); // Output: 3

// Assign default values
const [p, q, r, s = 0, t = 0] = numbers;
console.log(s); // Output: 4
console.log(t); // Output: 5
const [a , b , c , ...rest] = numbers;
console.log(a) // 1
console.log(b) // 2
console.log(c) // 3
console.log(rest) // [4 , 5]
```
## - Async 
It seems like you're requesting information about async functions. In programming, an async function is a type of function that allows asynchronous behavior. It is typically used when working with operations that may take some time to complete, such as fetching data from a remote server or reading from a file.

``` javascript
async function fetchData() {
  try {
    const response = await fetch('https://mohammadtamimi.com/data');
    const data = await response.json();
    return data;
  } catch (error) {
    console.log('Error:', error);
    throw error;
  }
}

fetchData()
  .then(data => {
    console.log('Data:', data);
  })
  .catch(error => {
    console.log('Error occurred:', error);
  });
```

