# JS Objects & DOM

## JS Objects

### What is an object ?
a set of variables and functions are grouped together to create a model.

### properties
in Objects, variables become known as properties.

### methods
in Objects, functions become known as methods.

### create an object using literal notation
literal notation is the easiest and most popular way to create objects.

```javascript
var hotel = {
  name: "name",
  rooms: 40,
  booked: 25,
  checkAvailabilty: function() {
    return this.room - this.booked;
  }
}
```
### accessing an object
you can access the properties and methods of an object using dot notation, or using square.
**dot notation**
```javascript
var hotelName = hotel.name;
```
**square**
```javascript
var hotelName = hotel['name'];
```

## DOM
This document object model allows access and modification of all document content.

### Dom Methods

**Examples dom methods**
- `document.getElementById()`
- `document.getElementsByTagName()`
- `document.getElementsByClassName()`
- `document.createElement()`
- `document.appendChild()`
- `document.write()`

### Change the Value of an Attribute
```javascript
document.getElementById(id).attribute = new value
```
