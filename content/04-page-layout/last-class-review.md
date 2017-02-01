+++
title = "Last Class Review"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/04-page-layout/agenda"
next = "/04-page-layout/code-along-1"
weight = 6

+++

## CSS Selectors Overview

- Many different types of selectors that allow you to target rules to specific elements in an HTML document

- Selectors are case sensitive, must match element names and attributes exactly

----

| Selector              |  Meaning                   | Example       |
|:---------------------:|:-------------------------- | :------------ |
| Universal Selector    | Applies to all elements    |      `*{}`
| Type Selector         | Match elements names       |  `h1, h2, h3 {}` |
| Class Selector        | Matches all elements with a class attribute value matching on specified after a period (.) | `.hint {}`, `p.hint {}` |
| ID Selector           | Matches all elements with a id attribute value matching on specified after a hash (#)      | ``#offer {}`` |
| Child Selector        | Matches elements that are a direct child of another | ``li > a {}`` |
| Descendant Selector   | Matches element that is a direct descendant of another (not just the child) | ``p  a {}`` |
| Adjacent Sibling Selector   | Matches first element that is a sibling of another | ``h1+p {}`` |
| General Sibling Selector   | Matches all elements that is a sibling of another | ``h1~p {}`` |
| Attribute Selector   | Attribute selectors select an element using the presence of a given attribute or attribute value | ``input[type="email"] {}`` |


{{% notice tip %}}
  A complete list of all CSS Selectors can be found [here](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
{{% /notice %}}


----

## CSS Box Model

- Understanding the CSS Box Model is key to understanding how CSS works

- Going forward, you should **view every element as a box** (because that's how browsers view them)

![inline](/images/03/box_model_example_no_lines.png)

![inline](/images/03/box_model_example_lines.png)

- Block elements in the image are outlined in red, while inline elements are outlined in green

- Every element is a box, some boxes contain other boxes ``<body>``, ``<div>`` or ``<article>``

- CSS allows you to create rules the control each individual box

<!--- Block elements (by default) start on the a new line | <body><p><h1> tags are examples of block elements-->
<!--- Inline elements Flow within the text and do not start on a new line Examples of inline elements include: <a>, <span>, <img>, <b>-->

----

### Box Model consists of:

- Margin

- Padding

- Border

![inline](/images/03/box_model_diagram.gif)


----

### Margin

- Margins sit outside the edge of your border

- Create a gap between the edges of two adjacent boxes


----

### Padding

- Padding is the space between the border of a box and any content contained within it.

- Adding padding helps to increase readability of a box’s content


----

### Border

- Every box has a border, even if it is invisible (0 pixels wide)

- Borders separates the edge of one box from another 
