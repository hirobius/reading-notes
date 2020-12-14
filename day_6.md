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

