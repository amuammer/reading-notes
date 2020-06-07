# JavaScript Head points

## Why we use JavaScript with Html ?
We use the JavaScript with html to make the web page dynamic <br/>
and do reactive actions with the page through it.

## Best for JavaScript code with Html
The best for JavaScript with Html to keep JavaScript code in its own JavaScript file with .js extension.

## JavaScript Linking with Html
HTML `<script>` element is used in HTML pages
to tell the browser to load the JavaScript file.
`<script src = "" > </script>`

## What is script ?
A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon. <br/>
```javascript
var today = new Date();
var hoursNow = todoy.getHours();
var greeting;
```

## JavaScript data types :
1. **string**
2. **number**
3. **boolean**
4. **undefined**
5. **null**
6. **object**
7. **array**
8. **function**


## JavaScript comments
* single-line comment <br/>
```javascript
var hoursNow = todoy.getHours(); // find the current hours
```
* multi-line comments
```javascript
/* this is
  multi line
  comment
 */
 var hoursNow = todoy.getHours();
```

# Html Text

## What is Html text elements ?
HTML elements are used to describe the structure of
the page (e.g. headings, subheadings, paragraphs).
```html
<!-- heading -->
<h1>heading</h1>
<!-- subheadings -->
<h2>subheadings</h2>
<!-- paragraphs -->
<p>paragraphs</p>
```
## Breaks and spaces
* To add white space in HTML you can use `&nbsp;` <br/>
* To add thematic break `<hr/>`
* To add break `<br/>`

# Introducing CSS

## What is CSS ?
CSS is used to control the style of a web document in a simple and easy way.

## CSS Syntax
You can put CSS Style Rule Syntax as follows <br/>
`selector { property: value }`

## CSS selectors
You can define selectors in various simple ways based on your comfort.
- Type Selectors
```css
h1 {
   color: #36CFFF;
}
```
- Universal Selectors
```css
`*` {
   color: #000000;
}
```
- Descendant Selectors
```css
ul em {
   color: #000000;
}
```
- ID Selectors
```css
#black {
   color: #000000;
}
```
