### What is redux
Redux is a predictable state container for JavaScript apps. As the application grows, it becomes difficult to keep it organized and maintain data flow. Redux solves this problem by managing application’s state with a single global object called Store.

### Redux Data flow

<img src="https://www.cronj.com/blog/wp-content/uploads/React-Redux.jpg" />

### What is an action
An action is a plain object that describes the intention to cause change with a type property. It must have a type property which tells what type of action is being performed

```JavaScript
const hideItems = () => ({
  type: "HIDE_ITEMS",
});

export const hideItemsAction = () => (dispatch) => {
  dispatch(hideItems());
};
```
### What is Redux Reducer
Actions and states are held together by a function called Reducer. An action is dispatched with an intention to cause change. This change is performed by the reducer. Reducer is the only way to change states in Redux,

```JavaScript
const initialState = {
  isVisible: false,
}

export default (state = initialState, action) => {
  switch (action.type) {
    case "HIDE_ITEMS": {
      return {
        ...state,
        isVisible: false,
      };
    }
  }
}
```

### setup redux
we do setup redux in index.js

```JavaScript
import logger from "redux-logger";
import thunk from "redux-thunk";
import { createStore, applyMiddleware } from "redux";
import { Provider } from "react-redux";
import reducer from "./redux/reducers/index";

const middlewares = [];
middlewares.push(thunk);
if (process.env.NODE_ENV !== "production") {
  middlewares.push(logger);
}

const store = createStore(reducer, applyMiddleware(...middlewares));

const hist = createBrowserHistory();

ReactDOM.render(
  <Provider store={store}>
    <Router history={hist}>
      <App />
    </Router>
  </Provider>,
  document.getElementById("root"),
);
```
