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

---

# JS Duckett (86-99)

Programmers use Methods, Functions and Objects to organize their code

---

## Functions

Let you group together statements to perform a specific task. 

Pieces of information passed to a function are known as **parameters**

When you write a function and you expect it to provide you with an answer, the response is known as the **Return Value.**

You can also have **anonymous functions** which don't have a name and as such can't be called but will instead run as soon as the interpreter comes across them. 

To create a function, you give it a name and then write the statements needed to achieve its task inside of the curly braces.

1. You **declare** a function using the `function` keyword.
2. You then give the function a name (sometimes called an identifier) followed by parentheses. i.e. `function doThis()`
3. The statements that perform the task sit in a code block / curly braces

The point to remember is that functions store the code required to perform a specific task, and that the script can ask the function to perform its task whenever and wherever needed. If different parts of a script need to perform the same task, you do not repeat the same statements, you simply use a function to do it.

The function can store the instructions for a specific task. When the function is finished running, the code continues to run from the point where it was initially called. (Sometimes you can call a function before it's declared, but this is some advanced ish.)

---

### Declaring functions that need information

Sometimes a function needs specific information to perform its task. In such cases, when you declare the function, you give it parameters. Inside the function, those words act like variable names. 

### Calling functions that need information

When you call a function that has parameters, you specify the values it should use in the parentheses that follow its name. The values are called **arguments**, and they can be provided as *values* or *variables.*

Parameters are the names of the values to ve filled in the function. The actual values or variables that fill the parameters are called arguments.

### Getting a single value out of a function

Some functions return information to the code that called them. For example, when they perform a calculation, they return a result.

The keyword **return** is used to return a value to the code that called the function. When the **return** is used, the interpreter leaves the function at that point. It then goes back to the statement that called it. If there were any subsequent statements in the function, they would not be processed. 

### Getting Multiple Values out of a Function

Functions can return more than one value using an **array**. 

### Anonymous Functions & Function Expressions

Expressions produce a value. If a function is placed where an expression is expected, then it gets treated as an expression. This is known as a **function expression**. (Study up on these...)

The interpreter always looks for variables and function declarations before going through each section of a script, line-by -line. This means that a function created with a function declaration can be ca lled before it has even been declared.

### Immediately Invoked Function Expressions (IIFE) pronounced "Iffy"

`var area = (function() {
  var width = 3;
  var height = 2;
  return width * height;
} ());`

The **Final Parentheses** after the closing curly brace of the code block tell the interpreter to run the function immediately.

The **Grouping Operators** (First and final parentheses), ensure the interpreter reads the included as an expression. 

IIFE's are commonly used for code that only needs to run once within a task, rather than repeatedly being called by other parts of the script.

### Variable Scope

The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's **scope**.

If you declare a variable within a function, it will only run within that function.

The interpreter creates local variables when the function is run, and removes them as soon as the
function has finished its task. This means that:
• If the function runs twice, the variable can have different values each time.
• Two different functions can use variables with the same name without any kind of naming conflict.

### How Memory and Variables work

Global Variables use more memory. Local variables are only remembered for the duration that they are needed during the execution of the function.

---

# 6 Reasons for Pair Programming

2 roles: the Driver and the Navigator.

Listening, Speaking, Reading and Writing

During a five-hour paired lab session, Code Fellows students work on all four of these language-specific skills. The abilities they foster will serve them well in completing assignments, in their own communication and learning, in interviews, and in readiness for a job at a company that utilizes this agile practice.

---

### Greater efficiency

Research indicates that pair programming takes slightly longer but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.

### Engaged Collaboration

When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. Another important aspect of learning to program is knowing when to ask for help. 

### Learning from Fellow Students

working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.

### Social Skills

When working with someone who has a different coding style, communication is key. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. When just grabbing the keyboard and taking over isn’t an option, getting good at finding the right words is a skill unto itself. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.

### Job Interview readiness

A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

### Work Environment Readiness

Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.


