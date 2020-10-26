# Motivation
When the application grows with more and more actions, the reducer function grows with it. We want to avoid large functions because they are difficult to overview, extend and combine.

There is a function called `combineReducer` that is shipped with Redux. It lets us split the reducer up to smaller reducers and combine them so we can use them in Redux.

# Let’s code our own combineReducer!

```JavaScript

// reducers.js
export default theDefaultReducer = (state = 0, action) => state;

export const firstNamedReducer = (state = 1, action) => state;

export const secondNamedReducer = (state = 2, action) => state;

// Use ES6 object literal shorthand syntax to define the object shape
const rootReducer = combineReducers({
  theDefaultReducer,
  firstNamedReducer,
  secondNamedReducer
});

const store = createStore(rootReducer);

```
