# Class 04 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## HTML & CSS Chapter 4: Links

Links are one of the defining features of web sites because they allow a user to quickly and easily travel from one web page to the next with a single click. There are several options to use when adding links to your web site. You can link to other pages on the same site, link to entirely new web sites, link to a different section of the same page or open up a new page in a new window. Links can also open up the users email program and add a specified recipient to the email form. Links use the `<a></a>` tags. Between the opening and closing `<a>` tag is where you add the destination to for the link, the visible name of the link and the `href` attribute, which stands for `hyper reference`. So if I want to add a link to `www.google.com`, it would look something like this:
```
<a href="https://www.google.com>GOOGLE</a>
```
This will display `GOOGLE` on the page and if you click on that it will direct you to google's home page.

Here are a couple of the modifiers to the `href` attribute:
* `href="mailto:'insert target email' ` This will open the user's email client and add the specified email into the recipient field
* `target="_blank"` adding this inside the opening `<a>` tag will open the link into a new page.

If you want to link to a different location on the same page, all you need to do is add an `id` selector to the html element you want the link to go to and simply replace the URL with the `id` selector like this:
```
<a href="#header"></a>
```

## HTML & CSS Chapter 15: Layout

Once you get past the basics of HTMl and CSS, the next step is thinking about the overall design of a page. In order to gain and keep traffic to your page, you need to make it appealing to users. One of the best ways to add some functional style to a page is by changing the layout. In HTML, elements are divided into two categories: block elements and inline elements. Block elements always start on a new line and take up the width of the page. Inline elements sit within text and other content and will not start a new line. Inline elements also typically can't have their height adjusted. There are a many different ways to approach layout. CSS has a few predefined positioning schemes:
* Normal Flow: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.
* Relative Positioning: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.
* Absolute positioning: This positions the element in relation to its containing element. Absolutely positioned elements move as users scroll up and down the page.
* Fixed Positioning: This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.
* Floating Elements: Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

In order to get block elements to sit side-by-side instead of the standard vertical, you can either float the elements in CSS:
```
section {
  float: left
}
```
or by the display property:
```
section {
  display: inline-block
}
```
These will position block elements next to each other, giving a different visual appeal other than having everything just in a vertical line.

One thing to keep in mind when designing the layout of a page is that not all devices have the same screen size or resolution. Make sure to take that in to account when positioning elements and assigning property values such as width in CSS. There are two standard types:
* Fixed width layouts: These will stay the same when a user increases or decreases browser window size.
Liquid layouts: These will adjust to fit the size of the browser window.

Both can have their advantages and disadvantages so it's important to know your audience when considering how your page layout is going to be designed.

## JavaScript and JQuery Chapter 3: Functions, Methods and Objects

Let's talk about JavaScript functions! We know how to write a basic script. But now we want more control, over those scripts. That's where functions come in to play. Functions are an extremely versatile, very important part of writing JavaScript. Functions take your code off of the global scope and encapsulate it inside of a function. First you must declare a function, `function 'give it a name'()`,
then using curly braces, `{}`, encapsulate your code below. Here's a small example of a basic function:
```
function howdy() {
     alert("This is a basic function!") 
}
```
When this function is called, it will popup with a notificaton saying 
>"This is a basic function!"

To call on a function, just add a HTML `<script>` tag and call the fucntion from the HTML document. That looks just like this:
```
<script>howdy()</script>
```
Simply use the name of the function, followed by (), and the script will run! By using functions, you can control when and where a JavaScript will run by using functions.

## Article: 6 Reasons for Pair Programming

What is pair programming? Pair programming is the concept that "two heads are better than one." Pair programing generally uses two positions, the driver and the navigator. The driver is the one actively writing code while the navigator is the one guiding the driver with input and direction without actually writing any physical code. With pair programming, a developer will listen, read, write and speak code: the four fundamentals to learning any new language, computer or lingual. There are several benefits to pair programming:

1. Greater efficiency: When two people focus on the same code base, it is easier to catch mistakes in the making. While pair programming may technically take a little longer up front, it will produce higher quality code that will need less fixing later on down the line. Ultimately, it's much more efficient than trying to have one person do everything step-by-step.

2. Engaged collaboration: When two people are working together, there is built in motivation and accountability to focus. 

3. Learning from fellow students: Since everyone thinks in a different way, pair programming can expose you to different ways to approach problem solving. If one developer is more skilled and is able to explain a concept to their peer, both parties will benefit. One of the best ways to learn a topic is to teach it to someone else.

4. Social skills
Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. 
This van have long-term career impacts. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.

6. Job readiness: A programmer who is versed in pair programming will be more hireable. Since it's a valued skill, it can often be used in interviews. Knowing how to work well in a pair programming environment will allow you to excel in this area. It will also show potential employers that you won't need to be trained in this area, making you a productive member of the team right out of the gate.