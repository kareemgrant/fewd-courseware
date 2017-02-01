+++
title = "Block and Inline Elements"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/04-page-layout/code-along-1"
next = "/04-page-layout/containing-elements"
weight = 9

+++

## Block Level Elements

- Always appear on a new line or row

- **By default**, block elements take up an entire row regardless of the width of their content

- Example block elements: `<p>`, `<h1>`, `<div>`

<a class="jsbin-embed" href="https://jsbin.com/zegoni/embed?html,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

{{% notice tip %}}
  Full list of block level elements can be found [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements)
{{% /notice %}}

----

## Inline Elements

- Sit within a block level element and do not start on a new line

- **By default**, inline elements only occupy the horizontal space needed to fit its content

- The height and width properties of an inline element will not be recognized

- Example inline elements: `<a>`, `<img>`, `<span>`


<a class="jsbin-embed" href="https://jsbin.com/xoxacaj/embed?html,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

{{% notice tip %}}
  Full list of inline elements can be found [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements)
{{% /notice %}}

----

## Inline-Block

- Allows you make an element inline while also allowing the element to recognize height and width properties

- inline-block is set as a value of the **display** property in CSS

<a class="jsbin-embed" href="https://jsbin.com/vocasel/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

----

## Changing Default Layout Behavior of Elements

- The default layout behavior of elements can be overriden using the **display** property in CSS

```
// in css

p.customer-logos {
  display: inline;
}

```

In the example above, we are using CSS to change the matching `<p>` elements (with a class of customer-logos) to display inline **instead of** its default display layout behavior of block


{{% notice tip %}}
  For more information about the display property click [here](https://developer.mozilla.org/en-US/docs/Web/CSS/display)
{{% /notice %}}
