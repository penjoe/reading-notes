# Class 02 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## HTML & CSS Chapter 2: Text

Chapter 2 of Jon Duckett's book *HTML & CSS: Design and build websites* covers the basics of text markup in HTML. Text is an integral part of many web pages as it is the bulk of the content provided for the user. Using various tags, text can be displayed in ways to emphasize certain parts and organize what the user is reading. One of the standard tags is the header tag, used to add a title to a page or a specific section. Using `<h1>` through `<h6>`, which are largest to smallest respectively, you can create headings, subheadings and even sub sub headings. Another vital tag is the `<p>` tag. This tag denotes a paragraph, or a block of text that is it's own individual block of content. Using tags, you can make text bold, `<b>` or italic, `<i>`. You can add subscript or superscript, `<sub>` and `<sup>` respectively, for added customization or emphasis. You can specify quotes, cite another authors work or specify and address:
* `<blockquote>` for large sections or `<q>` for smaller, inline quotes
* `<cite>` when citing someone's work
* `<address>` which is used to contain an specific physical or email address or telephone

These are some of the tags that can be used to add more customization and emphasis to HTML markup.

## HTML & CSS Chapter 10: Introducing CSS

Once a web page has been marked up with HTML, using CSS will allow you to add some color, change layout and really spice up your presentation. CSS operates by applying predefined style rules to specific HTML elements. By selecting an element you want to apply style to, you can change parts or all of a page with CSS rules. For example: 
```
body {
  background-color: blue;
  text-align: center;
}
```
This rule tells the browser to display the background of the `<body>` element blue and all text in the `<body>` element to align to center. While CSS rules can be applied using inline styling, meaning you add the CSS rules directly into the HTML, it's best to have an external .css file that you link to your HTML document with a link tag like this: 
```
<link href="style.css rel="stylesheet>
```
This tells the browser when it reads the HTML to go access the externally linked .css file and run the code there to apply styling to the HTML document. When writing CSS rules, it's always important to remember that it reads from top to bottom. After all, the CSS is short for Cascading Style Sheets. As it reads from top to bottom, it will always apply the last rule in the case of multiple rules for the same element. Or, if a specific element is selected by one of the various CSS selectors, such as the class or id selector, the browser will always apply the most specific rule. But once these basic rules are understood, CSS can be used to vastly change the appearance, and ultimately the end user experience of a web page.

## JavaScript & JQuery Chapter 2: Basic JavaScript Instructions

With JavaScript, a 'script' is just a set of instructions for the computer to follow to accomplish something. Each step in those instructions is known as a statement.A statement should always end with a semicolon. So what do we put in a statement? There are lots of components to JavaScript. Here are a few of the more important ones:
* Variables: basically storage containers to put things in
* Date Types: There are several, but a few of the basic ones are:
  * Numbers: as the name implies
  * Strings: a word os set of characters or numbers contained within quotations
  * Booleans: a true or false value
  * Null: an intentional blank value
  * Undefined: most often an accidental lack of value
* Arrays: Like a variable but it stores a list of values instead of just one
* Expressions: a method that evaluates into a single value

While there is a lot more to JavaScript than this , the above is a basic working list of what can go in to writing scripts. By using logic to combine various methods, you can create complex instructions for your computer to carry out to accomplish tasks both broad and very specific.

## ## JavaScript & JQuery Chapter 4: Decisions and Loops

Since we use conditional logic when writing JavaScript, there are often times where decisions are made that will determine what code will be run, if any. An simple example would be:
```
if (score > 50) {
  document.write('You passed!');
} else {
  document.write('Try again...');
}
```
In the above example, if the score is greater than 50, you get a message that tells you that you passed. If the score is not greater than 50, you get a try again message. `If a, then b, otherwise c.` Asl long as the logic makes sense, these decisions can get increasingly more complex, using multiple variables to store different values, various operators like 'less than', `<`, 'greater than', `>`,  or the `==` for 'equal to' operators. Once you understand the basics of logic and how operators help to make decisions, you can get more complex with loops. While comparison operators will often return a `true` or `false` value, logical operators will allow you to compare the results of more than one comparison operator. For example, `5 > 2` is a comparison operator. it's comparing if 5 is greater than 2. A logical operator will compare the results of different simple expressions into one, like this:
```
((5>2) && (2>=3))
```
This is comparing the results of the two individual expressions and producing one true or false value. There are three main logical operators:
* && - 'logical and' this tests more than one condition. It will always evalutate to false if at least one of its conditions value to false.
* || - 'logical or' this tests at least one condition. If either expression values to true, then the result will value to true.
* ! - 'logical not' this will take a single boolean value and invert it. It reverses the state of an expression.

The most important part of conditional logic is just to make sure that the logic being used makes sense. As it can get complex as more advanced scripts are written, this is very important to keep in mind.
