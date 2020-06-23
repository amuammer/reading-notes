# local Storage
localStorage property allows you to access a Storage object; <br/>
the stored data is saved across browser sessions; <br/>
localStorage properties allow to save key/value pairs. <br/>

### How to play with localStorage (CRUD)?
- **Creat** data in localStorage
```javascript
localStorage.setItem("key", "value");
```

- **Read** data from localStorage
```javascript
localStorage.getItem("key");
```
- **Delete** data from localStorage
```javascript
localStorage.removeItem("key");
```

### - **Hint**
if you store a number in localStorage, you need to parseInt the value after get it.
```javascript
const numberAsString = localStorage.getItem("number");
const number = parseInt(numberAsString);
```
