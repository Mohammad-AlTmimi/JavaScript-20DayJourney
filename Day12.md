# Day12
## - Practice
[SECTION'S EXERCISES](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week3-day1-tasks/tasks.md)
- Question 1
``` javascript
function convertStringToNumber(input){
  let ans = 0;
  let cnt = 1;
  for(let i = input.length - 1; i >= 0; i--){
      ans += (input[i] - '0') * cnt;
      cnt *= 10;
  }
  return ans;
}
```
- Question 2
``` javascript
function checkNaN(value) {
  return Number.isNaN(value);
}
```
- Question 3
``` javascript
function isEmptyValue(value) {
  return value === undefined || value === null || value === '';
}
```
- Question 4
``` javascript
function compareObjects(obj1, obj2) {
  if (typeof obj1 !== 'object' || typeof obj2 !== 'object') {
    return [obj1, obj2];
  }

  if (Object.keys(obj1).length !== Object.keys(obj2).length) {
    return false;
  }

  for (let key in obj1) {
    if (!obj2.hasOwnProperty(key) || !compareObjects(obj1[key], obj2[key])) {
      return false;
    }
  }

  return true;
}

```
- Question 5
``` javascript
function complexCoercion(input) {
  if (typeof input !== 'object') {
    if (typeof input === 'number') {
      return Boolean(input.toString());
    } else if (typeof input === 'string') {
      return Boolean(input);
    } else if (input === null || input === undefined) {
      return false;
    }
  }
  return input;
}
```
