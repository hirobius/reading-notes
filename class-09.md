# Chapter 7: “Forms” (p.144-175)
HTML forms give you a set of elements to collect data from
your users.

The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage

### Making Choices

Radio Buttons, Check Boxes, Dropdown Boxes

### Submitting Forms 

Submit Buttons, Image Buttons

### File upload

Allow users to upload files.

---

Users fill out forms, then submit info to a server.

The server processesthe information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.

The Server Creates a new page to send back to the user/browser based on the info received

---

For Controls live inside a `<form>` element. Every form element requires an `action` attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.

---

Forms can be sent using one of two methods: `get` or `post`.

---

With the post method the
values are sent in what are
known as HTTP headers. As a
rule of thumb you should use the
post method if your form:

●● allows users to upload a file

●● is very long

●● contains sensitive data
(e.g. passwords)

●● adds information to, or
deletes information from, a
database


---

Although the password is hidden
on the screen, this does not
mean that the data in a password
control is sent securely to the
server. You should never use
these for sending sensitive data
such as credit card numbers.
For full security, the server needs
to be set up to communicate
with users' browsers using
Secure Sockets Layer (SSL).

---

You can group related form
controls together inside the
`<fieldset>` element. This is
particularly helpful for longer
forms.
Most browsers will show the
fieldset with a line around
the edge to show how they are
related. The appearance of these
lines can be adjusted using CSS.

# Chapter 14: “Lists, Tables & Forms” (pp.330-357)

`list-style-type:`

`list-style-position` (Outside or Inside)


List Shorthand:
`ul {
list-style: inside circle;
width: 300px;}`

align numerals

shade alternate rows

hide empty cells

border collapse combines borders into 1

cursor styles


Styling input

`input {
font-size: 120%;
color: #5a5854;
background-color: #f2f2f2;
border: 1px solid #bdbdbd;
border-radius: 5px;
padding: 5px 5px 5px 30px;
background-repeat: no-repeat;
background-position: 8px 9px;
display: block;
margin-bottom: 10px;}
input:focus {
background-color: #ffffff;
border: 1px solid #b1e1e4;}`


# Chapter 6: “Events” (pp.243-292)

INTERACTIONS CREATE EVENTS 

EVENTS TRIGGER CODE

CODE RESPONDS TO USERS

### TERMINOLOGY

**EVENTS FIRE OR ARE RAISED**

When an event has occurred, it is often described as having fired or
been raised. In the diagram on the right, if the user is tapping on a link, a
click event would fire in the browser.

---

When the user interacts with the HTML on a web page, there are three
steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling.

1. Select the element
node(s) you want the
script to respond to.
2. Indicate which event on
the selected node(s) will
trigger the response.
Programmers call this binding an
event to a DOM node.
3. State the code you want
to run when the event
occurs. When the event occurs, on a
specified element, it will trigger
a function. This may be a named
or an anonymous function.

DOM event handlers were
introduced in the original
specification for the DOM.
They are considered better than
HTML event handlers because
they let you separate the
JavaScript from the HTML.

---

### Traditional DOM Event Handlers

Here is the syntax to bind an event to an element using an event handler,
and to indicate which function should execute when that event fires:

`element.onEvent = functionName;`

When using event handlers, the
event name is preceded by the
word "on" (onsubmi t , on change,
onfocus, onbl ur, onmouseover,
onmouseout, etc).

---

The addEventli stener ()
method takes three properties:
i) The event you want it to listen
for. In this case, the b 1 ur event.
ii) The code that you want it
to run when the event fires.
In this example, it is the
checkUsername (} function. Note
that the parentheses are omitted
where the function is called
because they would indicate that
the function should run as the
page loads (rather than when the
event fires).
iii) A Boolean indicating how
events flow, see p260. (This is
usually set to false.)

Unlike the HTML and traditional
DOM event handlers, when you
specify the name of the event
that you want to react to, the
event name is not preceded by
the word "on".
If you need to remove an event
listener, there is a function ca lled
removeEventL i stener(} which
removes the event listener from
the specified element (it has the
same parameters).

**Because you cannot have parentheses after the
function names in event handlers or listeners,
passing arguments requires a workaround.**

---

When an event occurs, the event object tells
you information about the event, and the
element it happened upon. The event object is passed to any function that is the event handler or listener. 

If you need to pass arguments to a named function, the event object will first be passed to the anonymous wrapper function (this happend automatically), then you must specify it as a parameter of the named function (as shown on the next page.)

When the event object is passed into a function, it is often referred to as e

---

If users can interact with a lot of
elements on the page, such as:
• a lot of buttons in the UI
• a long list
• every cell of a table
adding event listeners to each
element can use a lot of memory
and slow down performance.

By attaching an event listener
to a containing element, you are
only responding to one element
(rather than having an event
handler for each child element).

---

Whenever elements are added to or removed from the DOM, its
structure changes. This change triggers a mutation event.

When your script adds or removes content from a
page it is updating the DOM tree. There are many
reasons why you might want to respond to the DOM
tree being updated, for example, you might want to
tell the user that the page had changed.

### PROBLEMS WITH MUTATION EVENTS
If your script makes a lot of changes to a page, you
end up with a lot of mutation events firing. This can
make a page fee l slow or unresponsive. They can
also trigger other event listeners as they propagate
through the DOM, which modify other parts of the
DOM, triggering more mutation events. Therefore
they are being replaced by mutation observers.

### NEW MUTATION OBSERVERS
Mutation observers are designed to wait until a
script has finished its task before reacting, then
report the changes as a batch (rather than one at
a time). You can also specify the type of changes
.to the DOM that you want them to react to. But at
the time of writing, the browser support was not
widespread enough to use them on public websites.

---

The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.

Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.