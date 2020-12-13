# day 5

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

## Duckett: HTML & CSS, Chapter 10: Introducing CSS

A CSS rule contains two parts: a **selector** and a **declaration**. Declarations are split into two parts (a **property** and a **value**), and are separated by a colon. ie: ```p {font-family: Arial;}``` *(This rule indicates that all <p> elements should be shown in the Arial typeface.)*

elements can be combined with CSS rules. ie: ```h1, h2, h3 {font-family: arial; font-weight: bold; color: yellow;}``` 

CSS allows you to create rules that specify how the content of an element should appear. The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element. But in my case, we started by actually putting a 1pc border around everything to help with that.

Block level elements look
like they start on a new line.```<h1>``````<p>``````<div>```

Inline elements flow within the text and do not start on a new line. ```<b>``````<i>``````<img>```

The ```<link>``` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the <head> element. It should use three attributes:

```href``` the PATH to the CSS file
```type`` this specifies the type of document being linked to
```rel``` the "relationship" of the HTML file and what it is being linked to, in this case it's ```stylesheet```

(You can actually link multiple CSS files to a document, maybe use one for the presentation / fonts and colors and another for controlling layout!!! Genius.)

You can also include the CSS inside the HTML document itself by including your rules etc inside the Head of the HTML file inside of: ```<style type="text/css"></style>``` This is mostly only useful for static, single-page websites. Multiple page sites need an external.

CSS Selectors are case-sensitive.

Here are some more more in-depth looks at some CSS Selectors:

```* {}``` **Universal selector**, which targets all elements on a page

```h1, h2, h3 {}``` **Type selector**, which target specific elements

```.note {}``` **Class selector**, which targets any element whose attribute has a value of note. you can also do ```p.elementName {}``` to target only ```<p> ``` elements whose class attribute has a value of note

```#note``` **ID selector**, which can only be used once on a page. It targets the element whose id attribute has a value of note

```li>a {}``` **Child Selector**, which targets any ```<a>``` elements that are children of a ```<li>``` element (but not other ```<a>``` elements in the page.)

```p a {}``` Descent
 


## Lecture Notes: Cascading Style Sheets

* **Cascading:** Apply styles from top to bottom
* **Style:** Colors, size, position, layout 
* **Sheets** We can have multiple files

Every HTML tag has a style tag and can be applied inline, but it will override

The CSS box model is a great resource

Margin is how we make a box move around other boxes
Padding is how we move the the content inside of a box

When you use an id on a page, that's the only 

Class is a ".", id is "#"

The difference between an ID and a class is that an ID can be used to identify one element, whereas a class can be used to identify more than one.
