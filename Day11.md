# Day 11
## Practice
- [Exercises for Async JS & Promises](https://github.com/orjwan-alrajaby/gsg-expressjs-backend-training-2023/blob/main/learning-sprint-1/week2-day3-tasks/tasks.md)
## - Question 1:
``` javascript
const executeInSequenceWithCBs = (tasks, callback) => {
  const promises = tasks.map(task => {
    return new Promise(resolve => {
      task(message => resolve(message));
    });
  });

  Promise.all(promises)
    .then(messages => callback(messages))
    .catch(error => callback(null, error));
};
```
## - Question 2:
``` javascript
const executeInParallelWithPromises = (apis) => {
  const promises = apis.map(api => {
    return fetch(api.apiUrl)
      .then(response => response.json())
      .then(data => ({
        apiName: api.apiName,
        apiUrl: api.apiUrl,
        apiData: data
      }))
      .catch(error => ({
        apiName: api.apiName,
        apiUrl: api.apiUrl,
        apiData: null,
        error: error.message
      }));
  });

  return Promise.all(promises);
};
```
