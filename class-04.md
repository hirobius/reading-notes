# Chapter 4: Ch.4 “Links” (pp.74-93)

When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an absolute URL.

---

Relative URLS are links within the same site. You can use relative URLs which are a shorthand way to tell the browser where a page is in relation to the current page.

---

link to parent folder: 
`<a href="../index.html">Home</a>`

---

open in a new window:
`<a href="http://www.imdb.com" target="_blank">`

---

Before you can link to a specific part of a page, you need to identify the points in the page that the link will go to. You do this using the id attribute (which can be used on every HTML element)

To link to an element that uses an id attribute you use the `<a>` element again, but the value of the href attribute starts with the # symbol, followed by the value of the id attribute of the element you want to link to. In this example, `<a href="#top">` links to the <h1> element at the top of the page whose id attribute has a value of top:

`<h1 id="top">Film-Making Terms</h1>`

---

For different sites, you include links to specific parts of syntax that identify parts of a page. i.e. : 
to link to the bottom of the homepage of the website that accompanies this book, you would write:
`<a href="http:/www.htmlandcssbookcom/#bottom">`

---

# Chapter 15: “Layout” (pp.358-404)


