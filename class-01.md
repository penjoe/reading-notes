# Introductory HTML and JavaScript

[Home](https://penjoe.github.io/reading-notes/)

### Web Design Basics

Modern web pages use a combination of programming languages to display what the end user see in their browser. The three primary languages used for web pages are HTML, CSS and JavaScript. Each of the three languages have their own specific purpose. HTML provides the structure of the web page. This is the first thing the browser sees when you load a web page. Next, CSS adds styling to the HTML elements, adding visual appeal to a page. Finally, JavaScript adds function to a web page. These three languages together allow web developers to create visually appealing, dynamically functioning web experiences that the end user is able to enjoy simply by typing a web address into their browser. Lets take a look at how this all fits together.

### HTML and CSS

The first part of a web page is the HTML. This is the skeleton of the page that everything else layers onto. Using semantic tags, you can create a web page similar to how a newspaper would be layed out. There's a `<head>`, where basic page info is stored. Next is the `<body>` where you will add the bulk of the content. This can include a `<header>`, `<section>`, `<article>` and various other tags to mark up a frame to add onto. Here's a small example of a basic HTML structure:
```
<html>
	<head>
		<title>Page Title</title>
	</head>
    <body>
      <section>
        <h1>Section Header</h1>
        <p>Content goes here.</p>
        <p>More content goes here.</p>
      </section>
    </body>
</html>
```
In the example above, you can see that each element of HTML has an opening and closing tag with content in between them. While it can get much more complex as more code is added, the basic structure will ultimately stay the same. 

The above code example will appear very basic when loaded into a web browser. Using CSS, you can apply style to the HTML elements and give the page some character. This can be background color, font styles, and even page layout. Since we are using semantic elements in our HTML, it's very easy to specify what we want to style using CSS. For example, if we want to change the background of the body of the page, you could specify 
```
body {
  background-color: blue;
}
```
That would change the background color blue when you loaded in the web page. And with CSS, you can get as specific as you want using `class` and `id` attributes to specify specific elements of your HTML. Since adding tons of CSS to your document could end up getting very messy, it's always best to put all of your CSS into a separate file and link it to the HTML in the `<head>` element. 

Using HTML and CSS, you can create a structure and give it an appealing presentation that will keep users on your page and give them reason to come back in the future. Using JavaScript, you can add yet another layer to your web page to give it more life and make it much more user friendly. 

### JavaScript
Now that we know how to make a basic structure of HTML and give it some style with CSS, JavaScript will allow us to take the next step by adding dynamic functionality. A script is simply a set of instructions the browser will use to perform a task. Like a baker will follow a recipe for a cake, a web browser or computer will follow a script to do a thing. Here's a small example:

```
var greeting = 'Howdy ';
var name = 'Joe';
var message = ', please check your order:';
var welcome = greeting + name + message;
```
What the above script is doing is declaring variables for a welcome message. Variables? What are those? Variables act as storage containers in JS to store a value we want to use later. So `var name` means we are declaring that `name` is a variable. What will the value be that we are storing in `name`? Looking back up at the example, the value we are assigning to `name` is Joe. If the example script were to run, it would assign values to the first two variable and concatenate, or combine, those values into a third variable. Printing out the above script would end with 
>"Howdy Joe, please check your order."

JavaScript can also get complex as more lines of code is added, but as with any language, it's all done according to proper logic. And since it's read top down, we can know in what order a script will be run and where on the page it will run from. There are quite a few different things that can be done with JavaScript. But for now, we at least know the basics of what a script is and how it's used.

Using HTML, CSS and JavaScript together, you can create fun, dynamic web experiences that will keep your users engaged and give them reason to visit your page again in the future.

Check out my [GitHub](https://github.com/penjoe)!