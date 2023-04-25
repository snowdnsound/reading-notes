# Introduction to Web Development

##  Intro to HTML

There are six heading elements, starting with the largest h1 - h6.

HTML is the structure of the page, we need structure! This helps users scan the page quickly for information they need. It also helps severely visually impared people to use their screen reader to get information from the site. Search engines also use structure to return better indexing of your page. For example headers are considered more important. CSS also needs structure to target styling your page effectively.  

## JavaScript

CSS Declaration blocks are made up of CSS declatation pairs. These pairs consist of a property and a value. This allows you to affect an entire element on your page at once, as denoted by the selector. 

Operators in JS are used to produce results based on two values. 

Conditionals are code structures used to test if an expression returns true or not. For example if...else statements.  

Functions are a way of packaging up certain outputs that you wish to resuse and simplify your code.  

Events, are needed for interactivity on your site. Event headers listen for activity in your browser and then run code in response. 

Ex:  
document.querySelector("html").addEventListener("click", function () {
  alert("Ouch! Stop poking me!");
});  



## Questions From Reading

### HTML

Why is it important to use semantic elements in our HTML?

* So that it is intuitive to write code and for other people to read it and understand it.  

How many levels of headings are there in HTML?  

* There are six heading levels  

What are some uses for the sup and sub elements?  

* To be able to display dates and some scientific terms and math correctly on a page.  

When using the abbr element, what attribute must be added to provide the full 
expansion of the term?  

* The title atribute.   

### CSS

What are ways we can apply CSS to our HTML?  

* We can apply it internally, externally or in-line.  

Why should we avoid using inline styles?  

* Because it does not scale well and gets messy when you have a large website  

Review the block of code below and answer the following questions:  

What is representing the selector?  

* h2 is representing the selector, which tells the browser which element to affect.  

Which components are the CSS declarations?  

* The color and padding properties and their corresponding black and 5px value pairs.


Which components are considered properties?  

* Color and padding. 

### Learn JS

What data type is a sequence of text enclosed in single quote marks?  

* A string.

List 4 types of JavaScript operators.  

* +, addition  
* *, multiplication  
* =, assignment  
* !==, does not equal  

Describe a real world Problem you could solve with a Function?  

* You could use a function to add up all your walking steps for the week, and then have it tell you if you did more or less steps compared to last week.  

### Making Decisions in Your Code  

An if statement checks a __ and if it evaluates to ___, then the code block will execute?  

* Checks a condition, and evaluates to true. 

What is the use of an else if?  

* It give another option for the function if the condition evaluates as false.  

List 3 different types of comparison operators.

* ===, strict equality
* !==, strict non equality
* <=, less than or equal to

What is the difference between the logical operator && and ||?  

* For &&, AND operator, all expressions have to evaluate to true, for the whole expression to return true. For ||, OR operator, only one or more expressions have to evalauate to true, to return true. 


## Things I Want to Know More About

* JS and other syntax operators!