+++
title = "CSS Box Model"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/03-css-selectors-box-model/css-cascading-guidelines"
next = "/03-css-selectors-box-model/code-along"
weight = 13

+++

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

