## Event-Driven Programming in Node.js
Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a **click** event is triggered. When you press a key a **keydown** event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

## EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away.

```javascript
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```
