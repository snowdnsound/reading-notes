# Forms and JS Events

The five main elements to web forms are:

* form - this defines a form
* label - the name of the text field
* textarea - the input field 
* input - used to create interactive controls for the form
* button - used to submit their user data

It's important to mock up your form before you start coding. Try to keep your form to a minimum. Web forms allow users to interact with the site and us to collect data from them for a variety of reasons. 

Events are things that happen in the system you are programming, which the system tells you about so your code can react to them. Code can run automtacially based on an event that takes place. Here are some examples of events:

* The user selects, clicks, or hovers the cursor over a certain element
* The user chooses a key on the keyboard
* The user resizes or closes the browser window
* A web page finishes loading
* A form is submitted
* A video is played, paused, or ends
* An error occurs

To react to an event, you attach an event handler to it. This is a block of code is usually a JavaScript function that funs when the event fires. When a block of code is designated to run we call this registering an event handler. Event handlers are sometimes called event listeners. They are kind of interchangable but the listener listens out for the event happening, and the handler is the code that is run in response to it happening. 

Sometimes, inside an event handler function, you'll see a parameter specified with a name such as event, evt, or e. This is called the event object, and it is automatically passed to event handlers to provide extra features and information. 

## Things I Want to Learn More About

* Events
* Form libraries?
* Dark UI Patterns :/

## Handy Links

* [HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)
* [Your First Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)
* [Web Form Structure](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)
* [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
* [Intro to Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)
* [Form UX Design](https://www.smashingmagazine.com/2018/08/ux-html5-mobile-form-part-1/)
* [MDM Event Reference](https://developer.mozilla.org/en-US/docs/Web/Events)

## Questions From the Reading

### HTML Forms

Why are forms so important in web development?

* Because they allow us to interact and collect data from users. 

When designing a form, what are some key things to keep in mind when it comes to user experience?

* Make sure to use form validation so that it does not become a frustrating user experience. Also, don't make your forms too long. 

List 5 form elements and explain their importance.

* form - this defines a form
* label - the name of the text field
* textarea - the input field 
* input - used to create interactive controls for the form
* button - used to submit their user data

### Learn JS Events

How would you describe events to a non-technical friend?

* Events are ways the website responders to input from the user. 

When using the addEventListener() method, what 2 arguments will you need to provide?

* An argument that indicates what we want to listen to and a function to call when the event happens

Describe the event object. Why is the target within the event object useful?

* This is a parameter inside an event handler function, and can provide extra features and information. 

What is the difference between event bubbling and event capturing?

* Event bubbling starts firing events from the most nested elements to least, and event capturing starts firing events from the least nested to most nested. Event capture is disabled by default. 






