### React Props and State

## Components
 split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components.


## Stateful and Stateless Components

 Stateful and stateless components have many different names.

 They are also known as:

 – Container vs Presentational components

 – Smart vs Dumb components

 The literal difference is that one has state, and the other doesn’t. That means the stateful components are keeping track of changing data, while stateless components print out what is given to them via props, or they always render the same thing.

## React life cycles

#### Mounting
* componentWillMount
* render
* componentDidMount

#### Updating
* componentWillReceiveProps
* shouldComponentUpdate
* componentWillUpdate
* render
* componentDidUpdate

#### Unmounting
* componentWillUnmount
