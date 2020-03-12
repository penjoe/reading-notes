# Class 08 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## HTML & CSS Chapter 15: Layout 2.0

### Layouts

When styling a web page, one thing to take in to consideration is that not all users will be on devices with the same size browser window. Screen size can range anywhere from a smartphone all the way to a wide screen tv monitor. Because of this, it's common for web developers to create pages that are around 960 pixels wide. Most users will be able to properly see content this wide on their screens. 

Another consideration to make is what the user will see as soon as they load your page. What users see in the first couple seconds is what will determine if they will stay on your page or not. As a common design practice, developers will try to make sure that all of the information on the top ~600 pixels of the page is relevant and engaging. Often times, the bulk of the content will be below the browser window, so the goal is to make sure the top section of the page offers enough to entice users to scroll down. 

When considering layouts, there are two general categories:
* Fixed width layouts: These do not change if the user increases or decreases the size of their browser window. They will typically use pixel sizes.
* Liquid layouts: these will stretch and contract as the user increases or decreases the size of their browser window. They will typically use percentages.

Both types of layouts have their advantages and disadvantages. Fixed width layouts might have greater design control but might not be ideal on extra wide monitors or mobile devices. Liquid layouts will grow or shrink to fill a browser window but might make things distorted or harder to read if the browser window is really wide. While there is no right or wrong layout, it's important to take your targeted audience into consideration when styling a page.

When designing web pages, many web designers will use a grid to help them position items on a page. There are many possible layouts to choose one, but the industry standard is a 960 pixel wide, 12 column grid. With this, the width of the page is set, allowing easier styling knowing exactly how much space you have to work with. The columns help with spacing and placement.

### CSS Frameworks

CSS frameworks are pre-made CSS templates that can help save time by already having the code for things like layout grids, styling forms and such. The advantage of using a framework is that it will save a lot of time by limiting how much code you will need to write. They have also generally been tested across multiple device platforms and browser versions. The disadvantage of frameworks is that they will require specific class names in the HTML and often will contain way more code than is needed. 

### Stylesheets

Some web designers will create more than one style sheet for each project. One might be to control only the layout, another to control font, another to control colors etc. When linking multiple style sheets to the HTML, there are two ways to do so. 
* Use a separate `<link>` tag for each style page. 
* Link one style sheet and use `@import` to import other style sheets. The code for this is as follows:
```
//At the top of the CSS page that links to the HTML:
@import url('path to css file')
```
As with any CSS rule, it always reads top down. So even between linked pages, The last rule read by the browser will be the one to be applied.