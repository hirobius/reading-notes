# Chapter 6: “Tables” (pp.126-145)

Each block in the grid is referred to as a table cell. In HTML a table is written out row by row.

`<table>`
`<tr>`
`<td>`
`<th>`
`<td colspan="3">`

---

`<thead>`
`<tbody>`
`<tfoot>`


# Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

Object constructors can use a function as a template for creating objects
The name of the constructor function begins with a capital letter. This is to help remind developers to use the new keyword
The properties of each object are given as arguments to the function

To access a property of this
object, you can use dot notation,
just as you can with any object.

Similarly, to use the method,
you can use the object name
followed by the method name:
hotel.checkAvailability()

A variable has just one key (the variable name)
and one value.

Objects created with constructors are good when:
• You have lots of objects used with similar
functionality (e.g., multiple sl ideshows I media
players/ game characters) within a page
• A complex object might not be used in code

---

The DOM creates a model of the current webpage

The topmost object in the Document Object Model (or DOM) is the
document object. It represents the web page loaded into the current
browser window or tab.
the

DOM also creates an object for
each element on the page.

`document.createElement()` creates new element
`document . getElementByld()` returns element, if there is an element of the value id that matches

---

In JavaScript there are six data types:
Five of them are described as simple (or primitive) data types.
The sixth is the object (and is referred to as a complex data type).

1. String
2. Number
3. Boolean
4. Undefined (a variable that has been declared, but
no value has been assigned to it yet)
5. Null (a variable with no value - it may have had
one at some point, but no longer has a value)

6.0bject
Under the hood, arrays and functions are considered
types of objects.

Under the hood, JavaScript
treats every variable as an object in its own right.

FUNCTIONS ARE OBJECTS
Technically, functions are also objects. But they
have an additional feature: they are callable, which
means you can tell the interpreter when you want to
execute the statements that it contains.

---

The Math object has properties and methods
for mathematical constants and functions.

Because it is known as a global
object, you can just use the
name of the Math object followed
by the property or method you
want to access.

Using the floor () method
ensures that the number is
always rounded down to the
nearest integer, and you can
then add 1 to ensure the number
is between 1and10.

If you used the round () method
instead of the floor() method,
the numbers 1 and 10 would
be chosen around half of the
number of times that 2-9 would
be chosen.

---

Domain Modeling summary:

Summary
Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
Model its attributes with a constructor function that defines and initializes properties.
Model its behaviors with small methods that focus on doing one job well.
Create instances using the new keyword followed by a call to a constructor function.
Store the newly created object in a variable so you can access its properties and methods from outside.
Use the this variable within methods so you can access the object's properties and methods from inside.