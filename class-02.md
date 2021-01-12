# Stuff I didn't know:

## Text

**Line Breaks:** '''<br />'''
**Horizontal Rules:** '''<hr />'''

## Semantic Markup

**Emphasis:** '''<em>'''
**Blockquote:** '''<blockquote>'''>
**Abbreviations:** '''<abbr>'''
**Define:** '''<dfn>''' *(The first time you explain some new terminology)*
**Insert and Delete:** '''<ins>''' and '''<del>'''

Semantics are good because it can actually inform the browser on the contents of the page thus heightening its effectiveness.


# Introducing CSS

CSS Associates Style rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a **selector** and a **declaration.**

**Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.

**Declarations** indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.

---

**Properties** indicate the aspects of the element you want to change. For example, color, font, width, height and border.

**Values** specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.

--- 

## Selectors

* {} (Universal Selector)
h1, h2, h3 {} (Type Selector)
.note (Class Selector)
#note (ID Selector)
li>a {} (Child Selector)
p a {} (Descendant Selector)
h1+p {} (Adjacent Sibling Selector)
h1~p {} (General Sibling Selector)

---

### Test your code on diff. browsers

BrowserCam.com
BrowserLab.Adobe.com
BrowserShots.org
CrossBrowserTesting.com
PositionIsEverything.net
QuirksMode.org