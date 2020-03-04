# Class 03 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## HTML & CSS Chapter 3: Lists

When displaying a large portion of information, it can sometimes be hard to keep track of what is supposed to go where. Thankfully, HTML gives us the option to make lists. There are three types of lists to choose from:
1. Unordered lists: These lists use a bullet point system
2. Ordered Lists: These lists use a numbered system
3. Definition lists: These lists usually consist of a term or a concept followed by its definition.

Lists are a great way to group similar information together or to layout a step by step set of instructions. They an also be nested together, meaning you can have a list inside of a list. Here's a quick example of a list made with HTML:
```
<ul>
  <li>Mousses</li>
  <li>Pastries
    <ul>
      <li>Croissant</li>
      <li>Mille-feuille</li>
      <li>Palmier</li>
      <li>Profiterole</li>
    </ul>
  </li>
  <li>Tarts</li>
</ul>
```

## HTML & CSS Chapter 13: Boxes

The way CSS works, it views each HTML element as being in its own box. As such, it makes styling HTML elements somewhat predictable because we can have an idea of what all will be affected when we add styling. Boxes have 3 main properties to work with:
1. Border: this separates one box from the other
2. Margin: This is the space on the outside of the border
3. Padding: This is the space between the border and the content within

Using CSS, we can adjust those properties to control the size and even placement of a box. You can specifically adjust width or height or adjust one particular side of the box. CSS gives you a lot of control over how the "boxes" of HTML elements are displayed.

Aside from changing the size of a box, there are a lot of fun things CSS allows you to do. For example, you can make a solid border around a specific element, add a 3D style shadowing to a box, give it rounded corners and so on. Once you are able to control how boxes appear on the page, it gives you a lot of control over the overall page layout.

## JavaScript & JQuery Chapter 4: Decisions and Loops

We already went over basic conditional logic, such as if/else statements, and the various operators used to make decisions in JavaScript. The next step after that is loops. JavaScript has three types of loops:
1. `For loops` often used to loop through the items in an array. For loops will run a specified number of times.
2. `While loops` are used when you do not know how many times it will need to run. It will continue to loop until as long as the expression evaluates to true.
3. `Do while loops` are similar to while loops except that they will always run once, even if the expression evaluates to false the first time.

Loops, as the name implies, will continue to loop through a block of code until a specified condition is met. Operators can be used to help set these conditions. With this, if we need to get a specific result, we can have a loop continue to run until the required condition is met.
