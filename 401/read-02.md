# Read class 2

## What is TDD?

`TDD stands for Test Driven Development. The process is simple:`
<img src="https://miro.medium.com/max/700/1*-Qk4PaEr5CR6EQ3vhvRWyg.png" />


### ES2015 to ES6
```javascript
// es2015
function Rectangle(height, width) {
  this.height = height;
  this.width = width;
}
  // Getter
  Rectangle.prototype.area = function() {
    return this.calcArea();
  }

  // Method
  Rectangle.prototype.calcArea = function() {
    return this.height * this.width;
  }

// es6
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  // Getter
  get area() {
    return this.calcArea();
  }
  // Method
  calcArea() {
    return this.height * this.width;
  }
}
```
### ES6 this
`in ES6 if you want to access a property from any method you have to bind it`
```javascript
class Logger {
  constructor (name) {
    this.name = name;
    this.printName = this.printName.bind(this);
  }

  printName() {
    console.log(`Hello ${this.name}`);
  }

}
```

### ES6 inheritance
`in es6 you can do inheritance use extends`

```javascript
class Polygon {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}

class Square extends Polygon {
  constructor(sideLength) {
    super(sideLength, sideLength);
  }
  get area() {
    return this.height * this.width;
  }
  set sideLength(newLength) {
    this.height = newLength;
    this.width = newLength;
  }
}
