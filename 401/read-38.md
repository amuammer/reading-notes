# redux-thunk

## Introduction
By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects.


### Redux-Thunk
There are two very popular middleware libraries that allow for side effects and asynchronous actions: `Redux Thunk` and `Redux Saga`. In this course, we will explore `Redux Thunk`.

### setup redux-think
apply the middleware when creating your app’s store using Redux’s applyMiddleware

```javascript
import { createStore, applyMiddleware } from 'redux';
import thunk from 'redux-thunk';

const store = createStore(rootReducer, applyMiddleware(thunk));
```

### redux-think example
```javascript
import axios from 'axios';

export const addTodo = ({ title, userId }) => {
  return dispatch => {
    dispatch(addTodoStarted());

    axios
      .post(`https://jsonplaceholder.typicode.com/todos`, {
        title,
        userId,
        completed: false
      })
      .then(res => {
        dispatch(addTodoSuccess(res.data));
      })
      .catch(err => {
        dispatch(addTodoFailure(err.message));
      });
  };
};
```

### What if we don't want to use redux-think ?
```javascript
import axios from 'axios';

export const addTodo = ({ title, userId }) =>
  return new Promise((resolve,reject) => {
    axios
      .post(`https://jsonplaceholder.typicode.com/todos`, {
        title,
        userId,
        completed: false
      })
      .then(res => {
        resolve(res.data);
      })
      .catch(err => {
        reject(new Error(err.message));
      });
  };
```
