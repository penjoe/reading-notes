# Class 09 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## HTML& CSS Chapter 7: Forms

Form are useful to allow the user to submit information to the server which can then be returned back to the user via a new page depending on the information that was submitted. The submitted information is sent to the server in name/value pairs so that the date can properly correspond to its source. There are several form controls that provide different means for the user to submit their information. These controls offer specific types of form input. Here are some examples:
* Adding Text: 
  * Text input: allows user to input a line of text, like with the Google search bar
  * Password input: allows text input but obscures the characters entered
  * Text area: Allows a larger text field for submitting multiple lines, like a comment box
* Making Choices:
  * Radio buttons: allows user to select one of a multiple of options
  * Checkboxes: allows user to select and unselect one or more options
  * Drop-down boxes: gives the user a drop down list to choose from
* Submitting Forms:
  * Submit buttons: to submit data from your form to another page
  * Image buttons: similar to submit buttons, but with images!
  * File upload: allows user to upload files such as images

  Each of the above input options have their own corresponding html tag, but the parent tag will always be the `<form>` tag. As with a list, all the related tags that make up a form wil go inside of the `<form>` tag. Various form controls can also be labeled by using a `<label` tag, giving a name to the input field. 

  ## HTML & CSS Chapter 14: Lists, Tables & Forms

  Using CSS, you can control the look of lists, tables and forms. You can change or even remove the bullet point style in a list. You can add borders and colors to tables and individual cells within the table. With forms, you can style the look of the buttons, clean up the input fields and make sure they align perfectly and jazz them up to make them more user friendly. You can even change the look of the courser when a user hovers over a form. Each element used to make up lists, tables and forms can all be styled individually, giving you a huge array of customization options to play with.

  ## JavaScript and JQuery Chapter 6: Events

  When interacting with a webpage, a user can signal various events. When an event is triggered, a script can be run to respond to the event. There are many types of events that can occur while a user is browsing the web. Here a a few examples of common event categories:
  * UI events: Occur when a user interacts with the browser's UI, not the actual page
  * Keyboard events: Occur when user interacts with the  keyboard
  * Mouse events: Occur when the user interacts with a mouse, trackpad or touchscreen

  There are many other types of events that can be triggered, even ones that trigger when the DOM is manipulated. 

  How does triggering an event run JavaScript code? This is done in a process known as `event handling`.
  1. Select the element node to respond to
  2. Indicate which event will trigger the response
  3. State which code is run when the event is triggered

Events are bound to an element by event handlers. There are three types of event handlers:
* HTML event handlers: coded directly into the HTML element, this is considered bad practice and is an outdated handler
* DOM event handlers: manipulates the DOM via a function that is run. Only one function can be attached to an element. It looks like this:
```
element.onevent = functionName();
```
* DOM event listeners: a more recent approach, they can handle multiple functions but may not be supported by older browsers. Here's an example:
```
element.addEventListener('event', functionName, Boolean);
```

When dealing with events, it is important to understand the event flow. HTML elements nest inside other HTML elements. When an event is triggered, the element that event is tied to is inside of another element. There are two ways events can flow. The default is called `event bubbling`. This means that the event starts at the most specific node and flows outward. The other was is called `event capturing`. In this way, the event starts at the least specific node and works inward toward the most specific one. The flow of events primarily matters when an event handler is on an element and one of that elements ancestor or descendant elements. 
