
### What is JSX?

JSX stands for JavaScript XML.

JSX is an XML/HTML like extension to JavaScript.

` const element = <h1>Hello World!</h1> `

JSX is a XML syntax extension to JavaScript that also comes with the full power of ES6 (ECMAScript 2015).

Just like HTML, JSX tags can have a tag names, attributes, and children. If an attribute is wrapped in curly braces, the value is a JavaScript expression.

#### Learn Once, Write Anywhere

We don’t make assumptions about the rest of your technology stack, so you can develop new features in React without rewriting existing code.

#### Declarative

React makes it painless to create interactive UIs. Design simple views for each state in your application, and React will efficiently update and render just the right components when your data changes.

#### Component-Based

Build encapsulated components that manage their own state, then compose them to make complex UIs.

#### A Stateful Component

In addition to taking input data (accessed via this.props), a component can maintain internal state data (accessed via this.state)

#### Updating the Rendered Element

React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render().
