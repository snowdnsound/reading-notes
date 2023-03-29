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

An **external** style sheet must be saved with a .css extension. Here is an example of mystyle.css.

body {
    background-color: lightblue;
}

h1 {
    color: navy;
    margin-left: 20px;
}

**Note** Do not add a space between the property value and the unit!  
20px and not 20 px.

**With Internal**, this is used if one specific HTML page has a unique style. This is defined by the **style** element inside the **head** section of an HTML page. For example:

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

**Inline CSS**, may be used to apply a certain syple for a single element. To use this we add the style attribute to the relavant element. The style attribute can contain any CSS property. Example:  

<
h1 style="color:blue;text-align:center;">This is a heading(open arrow)/h(close arrow) 

**Note**

Inline looses many advantages of a style sheet, due to mixing contenet with presentation, so use this as least as possible.

## Multiple Style Sheets

If properties have been defined for the same selector element in different style sheets, the value from the last read style sheet will be used. So if a style for an element in an external stye sheet is defined before an internal style sheet, the value of the internal will apply. However, if the internal style is defined before the link to the external style sheet, then the value of the external will apply. 

**Cascading Order**

When there is more than one value specified for an HTML Element, all the styles will cascade into a new virtual style sheet by following the below rules in highest to lowest priority.

1. Inline style
2. External and internal style sheets
3. Browser default

## CSS Color Property

The color property specifies the color of text. Set the text color for different examples like so:

body {
  color: red;
}

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}



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
* [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
* [CSS Tools: Reset CSS](https://meyerweb.com/eric/tools/css/reset/)
* [Color Values](https://www.w3schools.com/cssref/css_colors_legal.php)

## Answer These Questions:

What is the purpose of CSS?

* It allows your website to look nicer and allows you to style your websites easier by applying site-wide rules.

What are the three ways to insert CSS into your project?

* With inline, external and internal style sheets.

Write an example of a CSS rule that would give all <p> elements red text.

* p {  
	color: red;  
}
