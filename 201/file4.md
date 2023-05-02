# HTML Links, JS Functions, and Intro to CSS Layout

## Handy Links

* [Creating Hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
* [Block vs Inline Elements](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#block_versus_inline_elements)
* [Link Text Best Practices](https://developers.google.com/style/link-text)
* [CSS Layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout)
* [Position Values](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
* [JS Functions](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)
* [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

## HTML Links

Hyperlinks are really important! they are what makes the World Wide Web an actual web. A basic link is created by wrapping the text or other content inside an <"a"> element and using the href attribute, also known as a Hypertext Reference, or target, that contains the web address. Typically you have block-level elements which form a visible block on a page, and inline-level elements, which are contained within block-level elements, and surround only small parts of the document's content. 

Hyperlink HTML  

<"p">
  I'm creating a link to
  <"a" href="https://www.mozilla.org/en-US/">the Mozilla homepage</"a">.
<"/p">

If you want to make a header element a link, do so by wraping it in an anchor link, such as below:  

<"a" href="https://developer.mozilla.org/en-US/">
  <"h1">MDN Web Docs</"h1">
</"a">
<"p">Documenting web technologies, including CSS, HTML, and JavaScript, since 2005.</"p">

It's imporant to follow link best practices when making them on your sites:

* Search engines use link text to index target files, so it is a good idea to include keywords in your link text to effectively describe what is being linked to.
* Don't repeat the URL as part of the link text — URLs look ugly, and sound even uglier when a screen reader reads them out letter by letter.
* Don't say "link" or "links to" in the link text — it's just noise. 

## Normal Flow & Positioning

Elements on a webpage lay out in normal flow by defualt, if you haven't applied any CSS to change the way they behave. Positioning allows us to produce interesting results by overriding normal document flow. For example maybe you have an element that you want to remain in the same place on page no matter where the user is.

Static positioning is the default of every element and just says to follow normal flow.

In your HTML:  
<"p" class="positioned">…</"p">

In your CSS rules document:  
.positioned {
  position: static;
  background: yellow;
}

Relative postioning is very similar to static positioning, except that once the positioned element has taken its place in the normal flow, you can then modify its final position, including making it overlap other elements on the page. You need to use the top, bottom, left, and right properties to modify the element. These declarations added below as an example. Note: The values of these properties can take any units you'd reasonably expect: pixels, mm, rems, %, etc.

position: relative;
top: 30px;
left: 30px;

Absolute positioning no longer exists in the normal document flow. These elements instead sit on its own layer separate from everything else. This is very useful: it means that we can create isolated UI features that don't interfere with the layout of other elements on the page. For example, popup information boxes, control menus, rollover panels, UI features that can be dragged and dropped anywhere on the page, and so on.

Top, bottom, left, and right declarations behave in a different way with absolute positioning. Rather than positioning the element based on its relative position within the normal document flow, they specify the distance the element should be from each of the containing element's sides. 

We can also have multiple layers outside of normal flow and we can contol what is on each layer with the z-index property. 

z-index: 1;  

Fixed positioning works in exactly the same way as absolute positioning, with one key difference: whereas absolute positioning fixes an element in place relative to its nearest positioned ancestor (the initial containing block if there isn't one), fixed positioning usually fixes an element in place relative to the visible portion of the viewport. An exception to this occurs if one of the element's ancestors is a fixed containing block because its transform property has a value other than none. This means that you can create useful UI items that are fixed in place, like persistent navigation menus that are always visible no matter how much the page scrolls.

## Functions vs Methods

Functions that are part of objects are called methods. The built-in code we've made use of so far come in both forms: functions and methods. You've also seen a lot of custom functions in the course so far — functions defined in your code, not inside the browser. This is better than having to write all that code out again every time we want to repeat it. And functions can contain whatever code you like — you can even call other functions from inside functions.





## Things I want to know more about

* [Accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility)
* [Built in Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)
* Arrow Functions

## Questions from the Reading Assignemnt

### Learn HTML

To create a basic link, we wrap text or other content inside what element?

* The "a" element <"a">. 

The href attribute contains what information?

* the web address that you want to send users to.

What are some ways we can ensure links on our pages are accessible to all readers?

* Follow best practices for link text, and use things like alt atributes to describe images.

### CSS Layout

What is meant by “normal flow”?

* This is the default way elements layout on a page if you don't alter it with CSS.

What are a few differences between block-level and inline elements?

* Block level elements affect an entire section or block of a page, whereas inline elements apply to small parts of the page's content

___ positioning is the default for every html element.

* Static

Name a few advantages to using absolute positioning on an element?

* You can have UI elements which are totally seperate and won't interfere with your normal flow elements
* It allows you to experiement with different elements on top of your existing ones


What is a key difference between fixed positioning and absolute positioning?

* Absolute positioning fixes an element in place relative to its nearest positioned ancestor and fixed positioning usually fixes an element in place relative to the visible portion of the viewport. 

### Learn JS

Describe the difference between a function declaration and a function invocation?

* Function declaration is creating the function, where as function invocation is recalling the function to run.

What is the difference between a parameter and an argument?

* A parameter is a value that needs to be included when invoking a function, arguments are the actual values that are passed to the function. 

### 6 Reasons for Pair Programming

Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.

* Greater efficiency - allows the code to be more accurate, with two sets of eyes on it. Which someone like me and customers could benefit from! 
* Learning from fellow students - Everyone has different perspectives and appraoches to a problem. This allows you too learn of new techniques or other methods in which to tackle the same issue. Also great for beginners and experts, gleaning knowledge and solidifying known concepts! 

