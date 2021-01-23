# Chapter 5: “Images” (pp.94-125)

CSS: `background-image` property

`<img src="images/quokka.jpg" alt="A family of
quokka" title="The quokka is an Australian
marsupial that is similar in size to the
domestic cat." />`

`src` tells the browser where to find the image
`alt` text desctiption which you cannot see, **helps search engines**
`title` is how you can some additional unseen info
`<img>` / images are actually inline elements

---

Use GIF or PNG format when saving images with few colors or large areas of the same color.
Jpegs for many color images

**bitmap:** tons of tiny squares

Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs or PNGs.

---

`<figure>` is used when you have an image + caption. Everything within the figure will share the same `<figcaption>`


# Chapter 11: “Color” (pp.246-263)

CSS3: HSL & HSLA Colors i.e. `hsl(0,0%,0%);`
HUE: 0-360 degrees
Saturation: %
Lightness: %
Alpha: 0-1

If using HSL, make sure you include hex code styles prior in case the older browser doesn't read the HSL value.


# Chapter 12: “Text” (pp.264-299)

If a font name is made up of more than one word, it should be put in double quotes when declared.
You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.

---

The default size of text in browsers is 16px. So **75%** is **12px**

---

A **pixel** `px` roughly equates to a **point** `pt` because a point corresponds to 1/72 of an inch.

---

#### 16px scale:

h1 32px
h2 24px
h3 18 or 16px
body 16px

---

You can also use pt for point sizes instead of px for pixels, but you should only do this when creating style sheets for printer friendly
versions of pages.

---

`@font-face` allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if
it is not on the user's machine.

---

### Font formats

Different browsers support different formats for fonts (in the same way that they support different audio and video formats), so you will need to supply the font in several variations to reach all browsers. If you do not have all of these formats for your font, you can upload the font to a website called FontSquirrel where they will convert it for you:

`eot, woff, ttf/otf, svg`

---

`text-decoration: blink`
This property is commonly
used by designers to remove
the underlines that browsers
place under links. Pages 290-291
show how to add or remove an
underline when a user hovers
over a link.

---

`line-height: 1.4em;` + `letter-spacing` + `text-indent`

---

When pseudo-classes are used, they should appear in this order: :link, :visited, :hover, :focus, :active.

# Attribute Selectors

***Study up on these...***

Existence`[]`

Equality`[=]`

Space`[~=]`

Prefix`[^=]`

Substring`[*=]`

Suffix `[$=]`