+++
title = "CSS Floats"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/04-page-layout/containing-elements"
next = "/04-page-layout/code-along-2"
weight = 15

+++

## Floating Elements


- Float property allows you to take an element in normal flow and place it as far to the left or right of the **containing** element as possible.
- Floats are a common way of creating multi-column layouts

----

## Floating Guidelines

- Floated elements should be assigned a width or unexpected behavior will occur (remember block level elements take up 100% width by default)

- Elements can be either floated **left** or **right**

- Elements that sit below will wrap around the floated element, it prevent this you must **clear the float**

----

## Adding floats using CSS

```html

blockquote {
  float: right;
  width: 275px;
}

```

**float** is a css property, the most common values are left and right


----

## Float Example

- Float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible

- Anything else that sits inside the containing element will flow around the element that is floated

<a class="jsbin-embed" href="https://jsbin.com/bezosuj/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

----

## Side by Side Example

- You can place blocks next to each other on the same line by setting the float and width properties on each block.

<a class="jsbin-embed" href="https://jsbin.com/kodifo/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

- Example: Each block of text is being floated to the left {float: left}, with the width set so multiple blocks can fit on the same line

- Potential issue: Paragraph #4 isn’t being displayed on a new line as expected. 

- Reason for this issue: Paragraph #3’s shorter height allowed another block to fit one line 1.

- Fix: using the **clear** property

----

## Clearing Floats Examples

- The clear property allows you to say that no element (within the same containing element) should touch the left or right- hand sides of a box 

- Accepts four values:

  - Left ({clear: left}): left-hand side of the box should not touch any other elements appearing in the same containing element.

  - Right ({clear: right}): right-hand side of the box should not touch any other elements appearing in the same containing element.

  - Both ({clear: both}): Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element. 

  - None ({clear: none}): Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.

<a class="jsbin-embed" href="https://jsbin.com/vuzuriz/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


----

## Parent Container Issue

- Some browsers treat containers of floated elements has having a height of 0 pixels tall.

<a class="jsbin-embed" href="https://jsbin.com/xewozo/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


- Example: We are attempting to add a border to the `<div>` that contains the three `<p>` elements

- Since all of the elements within the <div> are being floated, the browser treats it as if it has 0px height

- As a result, the border is not displayed correctly


----

## Parent Container Issue - Resolved

<a class="jsbin-embed" href="https://jsbin.com/nodufiw/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

- Multiple ways to fix this (here are a couple recommended approaches)

- Set overflow property to auto and set width to 100%

- You could just add a float property the containing `<div>`

