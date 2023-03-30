# Programming with JavaScript

**Control Flow** is the order in which the computer executes statements in a script.  

Code runs from the first line to the last line, unless it comes across conditionalal or loops.

A typical script in JavaScript incluedes many control structures including conditionals, loops and functions. Some parts might event run when certain events take place. 

## Functions

A JavaScript function is a block of code made to perform a certain task. A JavaScript function is executed when "something" invokes it (calls it). A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

* Function parameters are listed inside the parentheses () in the function definition  
* Function arguments are the values received by the function when it is invoked  
* Inside the function, the arguments (the parameters) behave as local variables  

The code inside the function will execute when "something" calls the function:

* When an event occurs (when a user clicks a button)  
* When it is invoked (called) from JavaScript code  
* Automatically (self invoked)  

When JavaScript reaches a return statement, the function will stop executing.  

If a function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.  

Functions often compute a return value. The return value is "returned" back to the "caller".

Functions are used because you can define the code one time and then reuse them.

## JavaScript Operators

* The Addition Operator + adds numbers  
* The Assignment Operator = assigns a value to a variable  
* The Multiplication Operator (*) multiplies numbers  
* The Addition Assignment Operator (+=) adds a value to a variable  

There are also different types of JavaScript operators:

* Arithmetic Operators - are used to perform arithmetic on numbers  
* Assignment Operators  - assign values to JavaScript variables  
* Comparison Operators  
* String Operators  
* Logical Operators  
* Bitwise Operators  
* Ternary Operators  
* Type Operators  

## JavaScript Comparison Operators

* ==	equal to  
* ===	equal value and equal type  
* !=	not equal  
* !==	not equal value or not equal type  
* ">	greater than"  
* <	less than  
* ">=	greater than or equal to"  
* <=	less than or equal to  
* ?	ternary operator  

All the comparison operators above can also be used on strings. The + can also be used to add (concatenate) strings as well as the += assignment operator can also be used to add (concatenate) strings. Adding two numbers will return a sum but adding a number and a string will return a string. 

## Logical Operators 

* &&	logical and  
* ||	logical or  
* !	logical not  

## JavaScript Type Operators and JavaScript Bitwise Operators

typeof	- Returns the type of a variable
instanceof	- Returns true if an object is an instance of an object type  

Bit operators work on 32 bits numbers. Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.




## Reference Links

* [Control Flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)  
* [Functions](https://www.w3schools.com/js/js_functions.asp  
)  
* [Operators](https://www.w3schools.com/js/js_operators.asp)  
* [PHP](https://developer.mozilla.org/en-US/docs/Glossary/PHP)  
* [Expressions & Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)  
* [More Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)  

## Questions To Answer

What is control flow?

* It's the order in which the computer executes statements in a script

What is a JavaScript function?

* A block of code designed to perform a particular task

What does it mean to invoke - or call - a function?

* This means to execute or run the function

What are the parenthesis () for when you define a function?

* The parenthesis are used to contain the parameters of the function
