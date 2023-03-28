# Design web pages with CSS



## Tips

* Chrome, right click Inspect > developer tools
* Other elements can nest inside an anchor tag, like an image

## How to Insert CSS

CSS is how you style your website, by controling how your HTML elements look in the browser. There are three different ways you can write CSS

* Internal - Seperate CSS file connected to HTML
* External - CSS is built into the HTML file
* Inline - CSS is built into the HTML, element itself

With external, you an change the whole look of a website by changing one file. External files are defined using the **link element** inside of the **head** section of an HTML page.  

An external style sheet must be saved with a .css extension. Here is an example of mystyle.css.

body {
    background-color: lightblue;
}

h1 {
    color: navy;
    margin-left: 20px;
}

**Note** Do not add a space between the property value and the unit!  
20px and not 20 px.

With Internal, this is used if one specific HTML page has a unique style. This is defined by the **style** element inside the **head** section of an HTML page. For example:

html
head
style
body {
    background-color: linen;
}

h1 {
    color: maroon;
    margin-left: 40px;
}
/style
/head
body

Inline CSS, may be used to apply a certain syple for a single element. To use this we add the style attribute to the relavant element. The style attribute can contain any CSS property. Example:  

<
h1 style="color:blue;text-align:center;">This is a heading(open arrow)/h(close arrow) 














We use classes & ID selectors to grab (select) the HTML elements.

selector {propterty: value,}
or  
selector {
    property: value;
}

selector {
    property: value;
}

selector {
    property: value;
    property: value;
    property: value;
}

## Positioning 

Static, relative, absolute & fixed




## Reference Links

* [What is CSS?](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)
* [How to Add CSS](https://www.w3schools.com/css/css_howto.asp)
* [CSS Color Property](https://www.w3schools.com/cssref/pr_text_color.php)

:43:08
