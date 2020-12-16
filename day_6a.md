# day_6a

###### [day_1](day_1.md)
###### [day_2](day_2.md)
###### [day_3](day_3.md)
###### [day_4](day_4.md)
###### [day_5](day_5.md)
###### [day_6a](day_6a.md)
###### [day_6b](day_6b.md)
###### [day_7](day_7.md)
###### [day_8](day_8.md)

###### [MASTER_NOTES.md](MASTER_NOTES.md)

# Read: 06a - Dynamic web pages with JavaScript

## Duckett: JavaScript & jQuery, Pages 43 - 69

The **document object** represents an HTML page.

Using the document object, you can access and change what content users see on the page and respond to how they interact with it.

The document object is just one of a set of objects that all major browsers support. When the browser creates a model of a web page, it not only creates a document object, but it also creates a new object for each element on the page. Together these objects are described in the **Document Object Model**.


The document object has:

1. **Properties** that describe characteristics of the current web page (such as the title of the page).

2. **Methods** perform tasks associated with the document currently loaded in the browser (such as getting information from a specified element or adding new content).

3. **Events** can be responded to, such as a user clicking or tapping an element.


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

—
## DoAlong — How do I write a script for a web page?

When possible, aim to keep the three languages in separate files, with the HTML page linking to the CSS and SavaScript files. Programmers often refer to this as a **separation of concerns**.


```<html>``` — Content Layer (Structure + Semantics)
```{css}``` — Presentation Layer (Rules + Presentation)
```javascript()``` — Behavior Layer (Interactivity)

These three layers form the basis of a web page building process called progressive enhancement.

—
## How to use objects & methods

This one line of JavaScript shows how to use objects and methods. Programmers refer to this as **calling** a method of an object.

The **document** object represents the entire webpage. All web browsers implement this object, and uou can use it just by giving its name.

```document.write('Good afternon!');```

—
## Member operator 
The **document** object has several methods and properties. They are known as **members** of that object. 

You can access the members of an object using a dot between the object name and the member you want to access. It is called a **member operator**. ```document.write```

The write() **method** of the **document** object allows new content to be written into the page 

There are tons of **objects** (ie ```document```) and methods (ie ```write('Good afternoon!'```)) that will help you write your own scripts.

JavaScript runs where it is found in the HTML, and where you put it will affect when it renders and page load times.


—
# Basic Javascript instructions

New vocab, new rules and new syntax!! Gotta love it. 

A script is a series of instructions that a computer can follow one-by-one. Each step or instruction is called a **STATEMENT**. Statements end with a ;

Javascript is case-sensitive.

Each STATEMENT should start on a new line and end with a semicolon. The semicolon tells the JavaScript **interpreter** (tool that translates the JavaScript) that it should move to the next step.

STATEMENTS can be organized into code blocks. The Code blocks are often used to group together many more statements which helps keep the code clean.

Use comments to explain what your code does!!! This will help make your code easier to read and understand. This will help everyone who touches it. 

Comment example:
```/* This is a multi-line comment that is used for longer comments. By closing the comment fully it prevents it from being registered by the interpreter */```

```// This is a single line js comment inside of a code block but in between statements (after the semicolon)```

—
## What is a variable?

Variables are used to store bits of information.

Variables can be used to represent values in your scripts that are likely to change. 

A variable is a good name for this concept because the data stored can change / vary each time a script runs.

This is similar to algebra, where letters represent numbers, but the = sign does something very different in programming...

—
## Variables: How to declare them

The process of creating a variable and giving it a name is called **declaring a variable**

Keywords are used in JavaScript to tell the interpreter to do something. ```var``` is a keyword. 

Variables must be named if you are to use them. i.e.: ```var quantity;``` camelCase is used if variable is longer than one word.

—

## Variables: Assigning them a value

Once a variable has been created, you then have to **assign it a VALUE** with an **assignment operator**

One assignment operator is the equals sign (=). This says that you are going to assign a value to the variable. ie: ```quantity = 3;```

## Data types

JavaScript distinguishes between **numbers**, **strings** and **booleans** *(true or false)*.

*(In addition to these 3 there are also **arrays**, **objects**, **undefined** and **null**)*

**Numbers** can also be negative (-123) or decimals (0.75).

**Strings** can also contain HTML markup. They must always be written on one line. You can use quotes inside of a string by using the opposite of either single or double quotes based what the string is contained in. You can also use a \ to inform the interpreter not to act upon the quotation mark.

**Booleans** are like a lightswitch... it's either on or off or 0/1


## Using a variable to store a number

Generally speaking, variables are first created, and then values are assigned to them and then they can be called upon at a later date.

## Using a variable to store a string

```
var username;
var message;
username = 'Molly';
message = 'See our upcoming range';
```

## Variable SHORTHAND

A bit more difficult to understand for beginners, but here:

```
var price = 5;
var quantity =14;
var total =price * quantity;
```

```
var price, quantity, total ; price =5;
quantity= 14;
total =price * quantity;
```

```
var price var total
5, quantity = 14; price * quantity;
```

``` 
 var el =document.getElementByld('cost'); 
 el.textContent ='$' +total;
```


## Changing the value of a variable

Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script!!

## Naming a variable

1. variables must begin with a letter, dollar sign or underscore. NOT NUMBERS

2. the name cannot contain dashes or a period.

3. you cannot use keywords or reserved words

4. case-sensitivty is a thing

5. use a variable name that describes the kind of information that the variable stores

6. Use camelCase