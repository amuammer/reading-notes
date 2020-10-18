# React Hooks

### What is a Hook?
A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.

### When would I use a Hook?
If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component. We’re going to do that right now!

### Hooks useState
In a function component, we have no this, so we can’t assign or read this.state. Instead, we call the useState Hook directly inside our component

```javascript
import React, { useState } from "react";

function Example() {
  // Declare a new state variable, which we'll call "count"  
  const [count, setCount] = useState(0);
}
```

### Effect Hook
The Effect Hook, `useEffect`, adds the ability to perform side effects from a function component. It serves the `same purpose` as `componentDidMount, componentDidUpdate, and componentWillUnmount` in React classes, but unified into a single API. (We’ll show examples comparing useEffect to these methods in Using the Effect Hook.)
