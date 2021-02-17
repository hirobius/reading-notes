# Docs for the HTML <canvas> element and Chart.js

## Chart.js API

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

---

### Setting Up

<https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/>

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script to the `<head>`:

`<script src='Chart.min.js'></script>`

---

Line, Pie and Bar Charts

---

Chart.js docs (important):  <https://www.chartjs.org/docs/latest/>

### Basic Usage

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.

The id attribute isn't specific to the <canvas> element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is always a good idea to supply an id because this makes it much easier to identify it in a script.

---

***You should always provide fallback content to be displayed by those browsers.***

---

`var canvas = document.getElementById('tutorial');
var ctx = canvas.getContext('2d');`

The first line in the script retrieves the node in the DOM representing the `<canvas>` element by calling the document.getElementById() method. Once you have the element node, you can access the drawing context using its getContext() method.

### Drawing Shapes

Unlike SVG, <canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths.

---

Rectangles, Paths, Moving the Pen, Straight Lines, Arcs, Bezier and Quadratic Curves, Shape Combinations, 

---

Line Width, Line Style, GlobalAlpha, Transparency, LineCap (Butt Round, Square), LineJoin, MiterLimit (The miterLimit property determines how far the outside connection point can be placed from the inside connection point.), Gradients (Linear, Radial, Conic), Patterns, Shadows, Fill, **Drawn Text**, Images, Frames from a Video, Scaling, Slicing (To Frame an image)
