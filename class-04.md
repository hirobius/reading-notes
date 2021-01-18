# Chapter 4: Ch.4 “Links” (pp.74-93)

When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an absolute URL.

---

Relative URLS are links within the same site. You can use relative URLs which are a shorthand way to tell the browser where a page is in relation to the current page.

If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.

---

link to parent folder: 
`<a href="../index.html">Home</a>`

---

open in a new window:
`<a href="http://www.imdb.com" target="_blank">`

---

Before you can link to a specific part of a page, you need to identify the points in the page that the link will go to. You do this using the id attribute (which can be used on every HTML element)

To link to an element that uses an id attribute you use the `<a>` element again, but the value of the href attribute starts with the # symbol, followed by the value of the id attribute of the element you want to link to. In this example, `<a href="#top">` links to the `<h1>` element at the top of the page whose id attribute has a value of top:

`<h1 id="top">Film-Making Terms</h1>`

---

For different sites, you include links to specific parts of syntax that identify parts of a page. i.e. : 
to link to the bottom of the homepage of the website that accompanies this book, you would write:
`<a href="http:/www.htmlandcssbookcom/#bottom">`

---

# Chapter 15: “Layout” (pp.358-404)

***Normal Flow***
***Relative Positioning***
***Absolute Positioning***
***Floats***

---

If one block-level element sits inside another block-level element then the outer box is known as the **containing** or **parent** element.

---

**Normal flow**
Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.

---

**Relative Positioning**
This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.

---

**Fixed Positioning**
This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.

---

**z-index property**
allows you to control which box appears on top.

---

**Relative positioning example:**
`p.example {
  position: relative;
  top: 10px;
  left: 100px;
}`

---

**Using Clear properly**

`body {
width: 750px;
font-family: Arial, Verdana, sans-serif;
color: #665544;}
p {
width: 230px;
float: left;
margin: 5px;
padding: 5px;
background-color: #efefef;}
.clear {
clear: left;}`

HTML:
`<p class="clear"></p>`

---

### Side note:

If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall.

to fix this in the CSS:
`overflow: auto;
width: 100%;}`

---

## CSS Frameworks

They are great for 
saving you from repeatedly writing code for the same tasks.
They are also often tested with different browsers.
These sometimes come with more code than you need *(Code bloat)*
Another disadvantage is that they often require that you use class names in your HTML code that only control the presentation of the page

# 960 Grid System

www.960.gs

Check these out too:

blueprintcss.org
lessframework.com
developer.yahoo.com/yui/grids/

# Multiple Style Sheets

1: Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.

`@import url("tables.css");`

or 

`<link rel="stylesheet" type="text/css" href="css/typography.css" />`