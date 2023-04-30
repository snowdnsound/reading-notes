# HTML Lists, Control Flow with JS, and the CSS Box Model

## Handy Links

- [Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) 
- [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
- [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

## Things I want to know more about

- Offline database of code rules somewhere? No Google?
- Nested Arrays, 2D, 3D?
- CSS transitions and animations
- [React](https://react.gg)
- Negative margins ?


## Questions from the Reading Assignemnt

### Learn HTML

When should you use an unordered list in your HTML document?

* When you have a list of items that you want to highlight, but don't need to be in a certain order.

How do you change the bullet style of unordered list items?

* Use the type atribute and give it a value of circle, disc, square or triangle. 

When should you use an ordered list vs an unorder list in your HTML document?

* When you need to have things listed in a speciic order

Describe two ways you can change the numbers on list items provided by an ordered list?

* Use the type atribute and assign a value of "i" to get Roman Numerals.
* Use the reversed atribute to reverse the number order. 

### Learn CSS

Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

* In this story called The Box Model the Margin character always plays it safe by keeping space between other elements on the website. The Padding character always remains best friends with the Content character. 

List and describe the four parts of an HTML elements box as referred to by the box model.

* Padding - space around the content, between the border
* Margin - outermost layer, space between other elements
* Border - goes around the content and the padding
* Content - the area your content is displayed in

### Learn JS

What data types can you store inside of an Array?

* Empty
* Mixed
* Nested

Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

* Yes it is, and you can use bracket notation along with the index number of the value you want to access like people[0][0] or people[1][2]

List five shorthand operators for assignment in javascript and describe what they do.

* (+) - adds two operands together
* ++ - adds 1 to operand
* -- - subtracts 1 from operand
* += - performs addition and assigns result to the left operand 
* -= - performs subtraction and assigns results to the left operand

Read the code below and evaluate the last expression and explain what the result would be and why.

* This will evaluate to 10, because false when added to 10 will convert to 0 due to type coercion.

Describe a real world example of when a conditional statement should be used in a JavaScript program.

* When needing to output a certain result based on new data input by a user. 

Give an example of when a Loop is useful in JavaScript.

* A loop is useful in order to write simpler and less code, or if you want to keep evaluating until a certain value is true.