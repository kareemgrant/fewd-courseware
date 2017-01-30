+++
title = "CSS Selectors"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/03-css-selectors-box-model/classes-and-ids"
next = "/03-css-selectors-box-model/css-cascading-guidelines"
weight = 11

+++

## CSS Selectors Overview

- Many different types of selectors that allow you to target rules to specific elements in an HTML document

- Selectors are case sensitive, must match element names and attributes exactly

&nbsp;

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
