# Class 01 Notes

World Wide Web    
Cient Requests >                <  Responses Server 



## Handy Links

[How the Web Works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)  
[JavaScript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)  
[Getting Started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)  
[HTML Data Structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)  
[Metadata in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)  
[DNS Lookup Tool](https://www.nslookup.io/website-to-ip-lookup/)  
[What is JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)  

## Questions from the Reading Assignment

### Getting Started

Compose a short poem describing how HTTP sends data between computers.

* The browser sends a message requesting a website to the server via HTTP  
To which the server agrees and sends the website for the client to see  
All of this is done via TCP/IP!  

Describe how HTML, CSS, and JS files are “parsed” in the browser.

* HTML is parced first, which then shows the browser if there are any link element references. It then sends back a request to the server for any CSS files it has found and any JavaScript files it has found from script elements. Then it parses the CSS or JacaScript. 

How can you find images to add to a Website?

* You can use sites like upsplash or stock photos to get images to use. 

How do you create a String vs a Number in JavaScript?  

* For a string you put single quotes around your data. For a number just put the number. 

What is a Variable and why are they important in JavaScript?  

* Variables allow you to store a value. These are important for doing more complex and interactive work on your website with a user. 

### Introduction to HTML

What is an HTML attribute?  

* This is 

Describe the Anatomy of an HTMl element.  

* You have an opening tag, a closing tag, and content in between

What is the Difference between <article> and <section> element tags?  

* Article encloses a black of text, for a blog post for example. Section is for multiple items that make up a single function or shared purpose on a site.  

What Elements does a “typical” website include?  

* Typically you have headers, p (paragraphs), ul (lists) (unordered and ordered), main, body, header, footer, and nav elements

How does metadata influence Search Engine Optimization?  

* It gives the search engine additional information because it is written in the search engine's language. 

How is the <meta> HTML tag used when specifying metadata?  

* You place it is the in the head section of an HTML page, and then place the attribute after it like "charset" for example  

### How to Start to Design a Website  

What is the first step to designing a Website?

* Figure out what exactly you want to accomplish first.  

What is the most important question to answer when designing a Website?

* Start with your goals and vision for the site, then figure out technical implementation. 

### Semnatics  

Why should you use an h1 element over a span element to display a top level heading?

* Because a header element is what search engines will prioritize to help your site be discovered and will size the heading properly. 

What are the benefits of using semantic tags in our HTML?

* Using semantic tags allows you to be able to code more intuitively and will help readers of your code more easily interpret your code.  

### What is JavaScript?

Describe 2 things that require JavaScript in the Browser?  

* Interactive or dynamic behavior on your site
* Store values inside varibales 

How can you add JavaScript to an HTML document?  

* You can add it internally with a script element, or externally with a JavaScript file (.js). 


## Pro Tips

Warning: Divs are so convenient to use that it's easy to use them too much. As they carry no semantic value, they just clutter your HTML code. Take care to use them only when there is no better semantic solution and try to reduce their usage to the minimum otherwise you'll have a hard time updating and maintaining your documents.