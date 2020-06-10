# Html

## links

* Links are created using the <a> element. <br/>
* The `<a>` element uses the **href** attribute to indicate the page you are linking to. <br/>
* If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.<br/>
* You can use the **id** attribute to target elements within a page that can be linked to.
* You can assign **target** attribute as blank if you want to open the link in a new tab.

## Layouts
* `<div>` elements are often used as containing elements to group together.
* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right
of the page and can be used to create multi-column
layouts.
* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.

## Functions

### What is function ?
group of a series of statements together to perform a specific task.

### Why we use function ?
* to make our code reusable
* to make our code more organized
* to save coding time

### Function Declaration
to create a function, you give it a name and then write the statements needed to achieve its task inside curly braces
- Declare a **function** using the **function** keyword
- Give the function **name**
- The **statements** that perform the task sit in a code block

```javascript
function sayHello() {
  document.write('Hello!');
}
```
* #### Declare function that need information
when you declare the function, you give it parameters inside the function, the parameters acts like variables

```javascript
function getArea(width, height){
  return width * height;
}
```

### Calling a function
execute all the statements of a function by just one line of code
```javascript
sayHello(); // function name
```

* #### calling function that need information
you can call a function that has parameters by specify the values in the parentheses that follow its name. The values called **arguments**

```javascript
getArea(3, 5);
```
