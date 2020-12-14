# day_6

###### [day_1](day_1.md)
###### [day_2](day_2.md)
###### [day_3](day_3.md)
###### [day_4](day_4.md)
###### [day_5](day_5.md)
###### [day_6](day_6.md)
###### [day_7](day_7.md)
###### [day_8](day_8.md)
###### [day_9](day_9.md)
###### [day_10](day_10.md)

###### [MASTER_NOTES.md](MASTER_NOTES.md)

# Read: 06a - Dynamic web pages with JavaScript

## Duckett: JavaScript & jQuery, Pages 43 - 69

**The document object.** represents an HTML page.

Using the document object, you can access and change what content users see on the page and respond to how they interact with it.

The document object is just one of a set of objects that all major browsers support. When the browser creates a model of a web page, it not only creates a document object, but it also creates a new object for each element on the page. Together these objects are described in the **Document Object Model**.


The document object has:

**Properties** that describe characteristics of the current web page (such as the title of the page).

**Methods** perform tasks associated with the document currently loaded in the browser (such as getting information from a specified element or adding new content).

**Events** can be responded to, such as a user clicking or tapping an element.


| EVENT | Happens when: |
| ----------- | ----------- |
| Load | Page and assets have finished loading |
| click | user clicks the mouse over the page |
| keypress | user presses down on a key |


| METHOD | What it does: |
| ----------- | ----------- |
| write() | adds new content to the document |
| getElementById() | Access an element when you state its id attribute |


## How a browser sees a webpage

1. Receive a page as HTML Code.
2. Create a model of the page and store it in memory. (beneath the document object each box is called a **node**. Each of these nodes is another object.)
3. Use a rendering engine to show the page on screen.

All major browsers read your JavaScript with an **interpreter** (or scripting engine). The interpreter translates the **interpreted programming language** language and processes each line of code one-by-one as the script is run.

Programmers can write code to say *"When this event occurs, run that code."*

## DoAlong — How do I write a script for a web page?

When possible, aim to keep the three languages in separate files, with the HTML page linking to the CSS and SavaScript files. Programmers often refer to this as a **separation of concerns**.


```<html>``` — Content Layer (Structure + Semantics)
```{css}``` — Presentation Layer (Rules + Presentation)
```javascript()``` — Behavior Layer (Interactivity)

These three layers form the basis of a web page building process called progressive enhancement.

## How to use objects & methods

This one line of JavaScript shows how to use objects and methods. Programmers refer to this as **calling** a method of an object.

The **document** object represents the entire webpage. All web browsers implement this object, and uou can use it just by giving its name.

```document.write('Good afternon!');```

### Member operator 
The **document** object has several methods and properties. They are known as **members** of that object. 

You can access the members of an object using a dot between the object name and the member you want to access. It is called a **member operator**. ```document.write```

The write() **method** of the **document** object allows new content to be written into the page 

There are tons of **objects** (ie ```document```) and methods (ie ```write('Good afternoon!'```)) that will help you write your own scripts.

JavaScript runs where it is found in the HTML, and where you put it will affect when it renders and page load times.


# Basic Javascript instructions

New vocab, new rules and new syntax!! Gotta love it. 

A script is a series of instructions that a computer can follow one-by-one. Each step or instruction is called a **STATEMENT**. Statements end with a ;

Javascript is case-sensitive.

Each STATEMENT should start on a new line and end with a semicolon. The semicolon tells the JavaScript **interpreter** (tool that translates the JavaScript) that it should move to the next step.

STATEMENTS can be organized into code blocks. The Code blocks are often used to group together many more statements which helps keep the code clean.

Use comments to explain what your code does!!! This will help make your code easier to read and understand. This will help everyone who touches it. 

Comment example:
```/* This script displays a greeting to the user based upon the current time. It is an example from JavaScript &jQuery book */```

```// This is a single line js comment inside of a code block but outside of a statement / after the semicolon```

