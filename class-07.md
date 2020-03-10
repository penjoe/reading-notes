# Class 07 reading Notes

[Home](https://penjoe.github.io/reading-notes/)

## Problem Domain

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem. Using object-oriented programming, you can create a hypothetical model of a problem, generate data, and create objects to store that data. Using a constructor function, you can make several object templates that can easily be updated with small, targeted changes as needed.


## HTML & CSS: Chapter 6 Tables

Tables can be created within an HTML document to help store and organize data. Tables are also useful when that data needs to be presented in a way that a user can easily find what they are looking for. Similar to  `<ul>` and `<ol>`, tables require just a few elements. Here's what a table looks like in HTML:
```
<html>
	<head>
		<title>Basic Table Structure</title>
	</head>
	<body>
		<table>
			<tr>
				<td>15</td>
				<td>15</td>
				<td>30</td>
			</tr>
			<tr>
				<td>45</td>
				<td>60</td>
				<td>45</td>
			</tr>
			<tr>
				<td>60</td>
				<td>90</td>
				<td>90</td>
			</tr>
		</table>
	</body>
</html>
```

This example would present a simple table of numbers that would look like this:
```
15	15	30
45	60	45
60	90	90
```
Here are the basic elements of a table:

* `<table></table>` all other tags related to the table go between these
* `<tr></tr>` these tags define a table row
* `<td></td>` these tags represent a new cell for the table
* `<th></th>` these tags represent a heading for a column or row


## JavaScript and JQuery: 

There are two ways to create an object. The first is called literal notation which was already discussed. The other is referred to as constructor function. Unlike literal notation, constructor notation uses a constructor function to make a template for an object that can then be populated with data using dot notation and bracket notation. So if we want to create an object called `hotel`, we would first make the constructor function.
```
var hotel = new Object();

hotel.name = 'Quay';
hotel.rooms = 40;
hotel.booked = 25;
```
This example would create a simple object called `hotel` with three properties, `name, rooms and booked`. The properties would have the values assigned to them by the dot notation. Using the constructor function, you can also make multiple objects at once.
```
function Hotel(name, rooms, booked) {
  this.name =  name;
  this.rooms = rooms;
  this.booked = booked;
}
```
Now we have a template for creating multiple objects as needed. Like in the previous example, we use the dot notation methind as well as the `this` and `new` keywords and simply fill in the blanks.
```
var quayHotel = new Hotel(`Quay`, 40, 25);
var parkHotel = new Hotel('Park', 120, 77);
```
This would give us two complete objects, one named `quayHotel` and the other `parkHotel`. Each object would have its own values based on the values entered. This way, if you need multiple objects all using the same format, you can create one function and then plug in multiple values. Objects can also be updated easily using dot notation after they have been created. 