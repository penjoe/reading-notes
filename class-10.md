# Class 10 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## JavaScript and JQuery Chapter 10: Error Handling & Debugging

When writing code, especially long or complicated scripts, errors are not at all unexpected. Part of programming is problem solving. When you run uo against errors, there are tools to help figure out what the error is and then solve the error. When searching for errors, it is important to take the order of execution into account. This is basically the processing order by which the computer runs scripts. This order of execution is then dependent on the scope of the script that is running. 

There are many different types of errors in JavaScript. These errors can often be identified using the console within the browser. Once an error has been identified, there are two ways to address it. 
1. Debug the script and fix any errors
2. Write a script that gracefully handles errors

Debugging is about deduction. Essentially, the debugging workflow is to find *where* an error is and then identify *what* and error is. While there is a lot more to it than that, it essentially boils down to those two steps. JavaScript has seven different types of errors. Each error creates its own error object to help identify where and what the error is. To help find where an error is, there are many developer tools available. One of the most common tools is the console, a built in tool in many modern browsers. There are also IDEs and programs designed to help with debugging. Once you find the error, break down the code that contains the error into smaller chunks so that you can test small pieces to help identify what is and is not working properly. 