# React life-cylces
<img src="https://camo.githubusercontent.com/af0801a9103f790cbdca1bee20df1f8055e36a33/68747470733a2f2f63646e2d696d616765732d312e6d656469756d2e636f6d2f6d61782f323030302f312a736e2d66746f7770305f565652626555414645434d412e706e67">

# Higher-Order Components

You may have used higher-order components, or HOCs, already. Redux’s `connect` function, for example, is a function that returns a HOC. But what exactly is a HOC?

**From the React docs:**
`A higher-order component is a function that takes a component and returns a new component.
`

Going back to Redux’s connect function, we can look at the following code snippet:

```javascript
const hoc = connect(state => state)
const WrappedComponent = hoc(SomeComponent)
```
When we call connect, we get a HOC back that we can use to wrap a component. From here we just pass our component to the HOC and start using the component our HOC returns.

**A good use case for an HOC is authorization. You could write your authentication code in every single component that needs it. It would quickly and unnecessarily bloat your code.**
