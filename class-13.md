# Class 12 Reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## Local Storage:

* no proper local storage for web apps historically
* HTML5 offered working solution via `localStorage()` object on the global window object
* HTML5 storage is based on key/value pairs
  * data is stored based on a key which can be retrieved via that key
  * data can be any JS data type, though actual data is stored as a string
* changes to local storage can be 'trapped', meaning the event attached to the window object
  * works similar to any other event
* max storage size via HTML5 is 5 megabytes
* two other competing options fot local storage:
  * 'Web SQL Database' is another solution to local storage, supported by major browsers
  * [The Indexed Database API](https://w3c.github.io/IndexedDB/)