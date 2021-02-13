# Onject Literals + DOM

## Chapter 3: “Object Literals” (pp.100-105)

Reading Skim:

`this` is a magic word in the magical world of Object Literals

Literal Notation is the easiest and most popular way to create objects.
Separating items with colons : and each property with a comma ,

---

There is a Variable, there are properties and then there are methods within that

---

You access the properties using "dot notation"

You can also create empty objects by leaving the curly brackets empty i.e. `let exampleOne = {}`
}

## Chapter 5: “Document Object Model” (pp.183-242)

Reading Skim:

The DOM is a separate set of rules
People often call the DOM an API (Application Programming Interface)
APIs let programs and scripts talk to each other

---

The DOM Tree is a model of a webpage, consists of 4 elements:

Document Nodes
Element Nodes
Attribute Nodes
Text Nodes

---

When you access any element, attribute, or text
node, you navigate to it via the `**document**` node. It is
the starting point for all visits to the DOM tree.

Every node is a descendant of the document node
Each node is an object with methods and properties.
Scripts access and transform the DOM tree, not the actual HTML

---

***To access the DOM tree, you start by looking for
elements. Once you find the element you want, then
you can access its text and attribute nodes if you
want to. This is why you start by learning methods
that allow you to access element nodes, before
learning to access and alter text or attributes.***

## Working with the DOM Tree

Accessing and updating the DOM tree involves two steps:
1: Locate the node that represents the element you want to work with.
2: Use its text content, child elements, and attributes.

Inconsistent browser support for the DOM was a key reason why jQuery became so popular.

---

The terms elements and element nodes are used interchangeably but when people say the DOM is working with an element, it is actually working with a node that represents that element.

---

Several methods let you create new nodes, add nodes to a tree, and remove nodes from a tree
This is called **DOM manipulation**.

---

Methods that find elements in the DOM tree are called DOM Queries
When you need to work with an element more than once, you should use a variable to store the result of this query.
This is known as **caching** the selection

`getElementById('One');` for example to access a node in some cases

---

You can access single items or lists

---

Nodelists look like arrays and are numbered like
arrays, but they are not ac tually arrays; they are a
type of object called a collection.

---

You can also loop and repeat actions to lists / collections

---

Array Syntax is preferred over the `item()` method because it is faster

---

## ACCESS & UPDATE A TEXT NODE WITH NODEVALUE

When you select a text node, you can retrieve or amend the content of it
using the `nodeValue` property.

---

You can access and change a text node and also update text with text content

---

## Adding or Removing HTML content

There are two very different approaches to adding anf removing content from a DOM tree: the innerHTML property and DOM Manipulation

---

You can also add elements to the DOM tree

---

If you add HTML to a page using i nnerHTML (or several jQuery methods),
you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise,
an attacker could gain access to your users' accounts. This book has several warnings about security issues
when you add HTML to a page using `innerHTML`.

---

You can also check for an attribute and get its values, also change them and remove them

---

End of chapter Summary:
*The browser represents the page using a DOM tree.
DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
Whenever a DOM query can return more than one
node, it will always return a Nadel i st.
From an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.
An element node can contain multiple text nodes and
child elements that are siblings of each other.
In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree .*

---

I will be needing a reread after lecture. sheesh!
