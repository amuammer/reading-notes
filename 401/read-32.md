# React Hooks

#### Five Important Rules for Hooks

Before we create our own Hook, let's review a few of the major rules we must always follow.

1. Never call Hooks from inside a loop, condition or nested function
2. Hooks should sit at the top-level of your component
3. Only call Hooks from React functional components
4. Never call a Hook from a regular function
5. Hooks can call other Hooks

#### React Hooks with Async-Await  
`We cannot use 'async' keyword with 'useEffect' callback method. It will result in race conditions.`

**We are fetching our books from google api and then updating our 'setResult' state with book title. React.useEffect method will only run when our 'searchBook' got change.**

```javascript
function useAsyncHook(searchBook) {
  const [result, setResult] = React.useState([]);
  const [loading, setLoading] = React.useState("false");

  React.useEffect(() => {
    async function fetchBookList() {
      try {
        setLoading("true");
        const response = await fetch(
          `https://www.googleapis.com/books/v1/volumes?q=${searchBook}`
        );

        const json = await response.json();
        // console.log(json);
        setResult(
          json.items.map(item => {
            console.log(item.volumeInfo.title);
            return item.volumeInfo.title;
          })
        );
      } catch (error) {
        setLoading("null");
      }
    }

    if (searchBook !== "") {
      fetchBookList();
    }
  }, [searchBook]);

  return [result, loading];
}
```

### Example of convert Class based Component to to Hooks
`class based`
```javascript

import React from 'react';

class Counter extends React.Component {
  constructor() {
    this.state = { count: 0 };
    this.incrementCount = this.incrementCount.bind(this);
  }

  incrementCount() {
    this.setState({ count: this.state.count + 1 });
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={this.incrementCount}>Click Me</button>
      </div>
    );
  }
}

export default Counter;
```
`to hOOks`
```javascript
import React, { useState } from 'react';

const Counter = () => {
  const [count, setCount] = useState(0);
  const incrementCount = () => setCount(count + 1);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={incrementCount}>Click Me</button>
    </div>
  )
}

export default Counter;
```
