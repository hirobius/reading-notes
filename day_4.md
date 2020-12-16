# day_4

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


## Duckett: HTML & CSS, Chapter 18 - Process & Design

* Design your website for the target audience.
* Creating personas can help infor your design decision making.
* Your content and design should be influenced by the goals and individual motivations of your users.
* You will need to provide key information based on you user's familiarity, goals and time.
* Different sites will need different levels of attention and upkeep to suit users' needs.
* When determining a sitemap, you are organizing the information at a higher level. During this phase, **card sorting** can be highly effective.
* When building out the individual page hierarchies, a wireframe exercise commences.
* Visual design is a tool for communication. Hierarchy, grouping and similarity.
* You can differentiate between pieces of information using size, color, and style.
* Grouping and similarity can help further simplify the info you're trying to convey.
* Web users SKIM the page. Visual hierarchy is key as it helps you skim efficiently.
* Navigation should be **concise, clear and selective**. 


## Duckett: HTML & CSS, Chapter 17 - HTML5 Layout

* New HTML elements in HTML5 make the content easier to follow, help screen readers, enhance search engines and help web authors more efficiently describe the structure of the page.
* An ```<aside>``` is usually filled with info related to the element it is within.
* Sections help divide up the page, but should not be used for containing the entire page, a ```<div>``` is best for that.
* ```<hgroup>``` can be used to group / sort both a heading and subheading together in the same element.
* ```<figure>``` elements *(images, videos, graphs etc...)* almost always come with a ```<figcaption>``` element.
* Anything that lies outside of the ```<header>``` ```<footer>``` or ```<aside>``` elements can be considered the main content and don't need a ```<content>``` element to house them.
* With HTML5, it is now considered permissible to link an entire block with the ```<a href>``` element.
* In order to help old browsers, it is proper to include a line of CSS like the following to call out which elements are to be displayed in block format instead of inline: ```header, section, footer, aside, nav, article, figure {
  display: block;}```
* all in all, the new elements just provide clearer code.


## Duckett: HTML & CSS, Chapter 8 - Extra Markup

* ```<!-- -->``` to comment.
* The id attribute is a global attribute as it can be used on anything.
* Every HTML attribute can also carry a class attribute
* Block elements are elements that always appear on a new row such as: ```<h1>``` ```<p>``` ```<ul>``` etc.
* Divs can be good for containing entire sections of a page. Often times when you close a div it is often to add a comment.
* A ```<span>``` element acts like an inline equivalent of a ```<div>```
* An ```<iframe>``` is actually a window into another webpage
* The ```<meta>```  element lives inside the ```<head>``` element and contains information about that web page. It can house some pretty intricate info that goes unseen on the webpage as it does things like informing search engines about the page's contents, whether or not it is time sensitive or who created the page. It does not have a closing tag. 
* Escape characters, or a combination of other characters, are used to create special characters. 