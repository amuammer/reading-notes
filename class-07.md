# Html Tables and JavaScript Objects

## Html Tables

### What is a table ?
a table represents information in a grid format.

### Basic table structure
- `<table>` element used to create a table
- `<tr>` element used to create a table row
- `<td>` element used to add data to the table row
- `<th>` element used just like `<td>` but its purpose to represents the heading

### spanning
some times you may need the entries in a table to strech accross more than one column or row <br>
span attribute can be used on a `<th>` or `<td>`

- `<td colspan="2" >` to span col across 2 columns
- `<td rowspan="2">` to span down 2 rows

### long tables
elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).

- `<thead>` headings of the table should sit inside this element.
- `<tbody>` The body should sit inside this element.
- `<tfoot>` The footer belongs inside this element.

## JavaScript Objects

### What are built-in Objects:
The three sets of built-in objects each offer a different range of tools that help you write scripts for web pages.

### Browser Object Model:
- **Browser Object Model:** The Browser Object Model creates a model of the browser tab or window. <br>
The topmost object is **window** object, which represents current browser window or tab, its child objects represents other browser feature.

**Window** current browser window or tab. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-- **Document** current web page. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-- **History** pages in browser History. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-- **Location** Url of current page <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-- **Navigator** information about browser <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-- **Screen** device's display information <br>

**Examples** <br>
`window.alert()` <br>
`window.screen.width` <br>

### Document Object Model
- **Document Object Model:** The Document Object Model (DOM) creates a model of the current web page. <br>
The topmost object is the **document** object, which represents the page as a whole. its child objects represent other items on the page.

**Examples** <br>
`document.getElementById();` <br>
`document.lastModified;` <br>

### Global JavaScript Objects
- **Global JavaScript Objects:**
The global objects do not form a single model. <br>
They are a group of individual objects that relate to different parts of the JavaScript language.

These objects represent basic data types: <br>
**String** For working with string values. <br>
**Number** For working with numeric values <br>
**Boolean** For working with boolean values. <br>

These objects help deal with real-world concepts: <br>
**Date** to represent and handle dates <br>
**Math** for working with numbers and calculations <Br>
**Regex** for matching patterns with strings of text <br>

**Examples** <br>
`hotel.toUpperCase();` <br>
`Math.PI;` <br>
