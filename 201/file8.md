# CSS Layout

## Flexbot

The Flexible Box Layout Model (flexbox) is a layout model designed for one-dimensional content. It excels at taking a bunch of items which have different sizes, and returning the best layout for those items. Flexbox not only helps lay the sidebar and content out inline, but where there's not enough space remaining, the sidebar will break onto a new line. Instead of setting rigid dimensions for the browser to follow, with flexbox, you can instead provide flexible boundaries to hint how the content could display.

You can do the following with a flex layout:

* Display as a row, or a column.
* Respect the writing mode of the document
* They are single line by default, but can be asked to wrap onto multiple lines
* Items in the layout can be visually reordered, away from their order in the DOM
* Space can be distributed inside the items, so they become bigger and smaller according to the space available in their parent
* Space can be distributed around the items and flex lines in a wrapped layout, using the Box Alignment properties
* The items themselves can be aligned on the cross axis

When elements are laid out as flex items, they are put along two axis. The main axis is the axis running in the direction the flex items are laid out in (for example, as a row across the page, or a column down the page.) The start and end of this axis are called the main start and main end.
The cross axis is the axis running perpendicular to the direction the flex items are laid out in. The start and end of this axis are called the cross start and cross end.  

The parent element that has "display: flex" set on it (the <"section"> in our example) is called the flex container.
The items laid out as flexible boxes inside the flex container are called flex items (the <"article"> elements in our example).

Previously the following were difficult or impossible to achive with float:

* Vertically centering a block of content inside its parent
* Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available
* Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content

## Things I want to know more about

* Flexbot and card components 

* Flex-flow shorthand

## Handy Links
* [CSS Flexbox](https://web.dev/learn/css/flexbox/)

* [CSS Layout Flexbot](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

* [Typical Use Cases of Flexbot](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Typical_Use_Cases_of_Flexbox)

## Questions from the Reading

### Learn CSS

Flexbox is designed for one-dimensional content. Explain what this means?

* This means that it only works on a single plane and does not use the z-index 

Explain the difference between the main axis and cross axis?

* The main axis is the axis running in the direction the flex items are laid out in, and cross axis is running in the directino perpendicular to the flex items, like an x and y axis. 

How can using certain properties of flexbox negatively impact accessibility?

*  Flexbot can increase loading times which could impact people accessing your website.

### CSS Layout

What are some advantages of using flexbox over float?

* It is more "flexible" to work with in terms of allowing items to have the same space between them, especially columns and vertical centering.

How does this topic connect with your long term goals?

* I think flexbot will help with designing UI elements and card layouts on websites, which is a part of what I would want to build. 