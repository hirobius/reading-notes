# Introduction (pg. 2-11)

## The book is divided into 3 sections: 

1. HTML *(Structure)*
2. CSS *(Presentation)*
3. Practical

There are also other goodies in the book like SEO, using Analytics software, design techniques and other miscellaneous items.

## Terminology

Browsers: Software people use to access a website
Web Servers: Special computer that hosts the website and receives requests from the browser
Devices: All kinds of em.


## How the Web Works

In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.

You connect to the web through an **ISP** / Internet Service Provider.

You type a domain name / web address into your browser to visit a site.

Your computer then contacts a network of servers called a DNS / Domain Name System. (These act like phone books and tell your computer the IP address associated with the requested domain name.) IP addresses are up to 12 characters long separated by periods.

The unique number that the DNS server returns to your computer allows your browser to contact the web server.

The web server then sends the page you requested back to your browser.


# Chapter 1: Structure (p. 12-39)

The key takeaway in the beginning of the chapter is that it is important to have a hierarchy of information.

HTML is key to building out the structure of a webpage. 

HTML uses tags to give pieces of content special meaning. (Tags are like containers and usually come in pairs)

Opening tags can carry attributes, which tell us more about the content of that element.

Attributes require a name and a value.

To learn HTML, you need to learn what tags are available, where they can be used and what they actually do.

[Go Here](www.htmlandcssbook.com/code/) and view source to look at some sample code for this chapter.


# Chapter 8: Extra Markup (p. 176-199)

There have been new versions of HTML and new browsers that support these new features.

Because of these new versions of HTML, each webpage must declare a Doctype explaining what version of HTML is being used.

Comments are written in HTML like this: '''<!-- comment goes here -->''' pretty neat.

**Every HTML element can carry the ID attribute.** The main rules here are that its value should start with a letter or an underscore, not a number or any other character. It is also important to note that no two elements on the same page can have the same value for their id attributes. (Otherwise the value is no longer unique.)

When using javascript, id attributes can be used to allow the script to work with that particular element.

**Class attributes** are applied to groupings of elements and can be applied more broadly.

**Block elements** always start a new line when used. i.e. '''<p>''' '''<h1>''' '''<ul>''' etc...

**Div elements** allow you to group a set of elements together in one "block-level" box. Divs can also make it easier to follow the content of your page if it is tastefully divided into different sections with divs. Since there may be several other elements inside a <div> element, it can be helpful to add a comment after the closing </div> tag.

**Span elements** are the inline equivalents of divs. They are most commonly used to control the look of inline text by using CSS to affect the span class surrounding the text to be altered.

**meta** element lives inside the Head and containg info abut the page. Info such as who made it, if it is time sensitive, and search engine info. Some defined values for this are **description** or more interesting ones like **pragma** which prevents browsers from caching the page. Pretty much lets you supply all kinds of information about your page.

**Escape characters** are those that don't natively show up like ampersands or the copytright symbol that must be shown using a code / series of characters.

# HTML5 Layout (428-451)

There are new HTML layout tags that are more explicit in their function than relying on Divs to set the page up.
Side note: Header and Footer elements can be used in individual article or section tags within the page.

**hgroups** are used to group together header stylings
**figure** tags are used to refer to content such as images or videos and also contains a fig caption

You can add links around entire blocked elements
In order for pages before IE8 to work you may need some additional HTML shiv javascript (hosted on google).
Also, apparently conditional comments are a thing! 

# Process & Design (p. 452-475)

Sitemaps, Wireframes, Visual Hierarchy, Grouping / Gestalt Principles. Design is about communication.

---

# Duckett JS Intro.

JS makes websites more interactive, interesting and User-friendly. Also, JQuery helps make writing JavaScript a lot easier.

Learning javascript requires 3 basic things:

1. Understand some basic programming concepts and the terms that Javascript developers use.
2. Learn the language and vocabulary itself and how to properly form "sentences" in this language.
3. Become familiar with how it is applied by looking at examples of how javascript is commonly used in websites.

You can use JS to **access** any element, attribute, or text from an HTML page. JS can also **modify** these elements or attributes. You can also **progam** rules and make the page **react** to certain events. 

---

HTML Elements are added to a page to describe its structure. An **element** consists of its opening (may include attribute names and values) and closing tags and the content between the tags.

CSS rules i.e. '''.fruit {color: pink;}''' include CSS selectors which are affected by properties and their values. Each declaration in the declaration block has a property (the aspect you want to control) and a value, which is the setting for that property.

# The ABCs of Programming

- What is a Script and how do I create one?
- How do computers fit in with the world around them?
- How do I write a script for a web page?

### What is a script and how do I create one?

To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.
