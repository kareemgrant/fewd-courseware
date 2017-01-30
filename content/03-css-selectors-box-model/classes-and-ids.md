+++
title = "Classes and Ids"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/03-css-selectors-box-model/css-intro-review"
next = "/03-css-selectors-box-model/css-selectors"
weight = 9

+++

## Classes and Ids

- Both are just HTML attributes

- Should start with a letter or underscore

- Can be applied to any html element

- **Important:** Use of the class or id attribute by itself does not change the appearance of an element; CSS/Javascript must be involved

&nbsp;

## Class Attribute

- Is used to group elements together, therefore establishing them as different from other elements on the page

- Element can share the same class attribute values (this could be applied to another type of element)

```
  <!-- in html -->

  <p class='important'> Awesome content </p>

```


```

  // in css, use a period to specify a class selector in css

  .important {
    font-weigth: bold;
  }


```

{{% notice tip %}}
  In css **class** selectors are specified using a ``.`` (period)
{{% /notice %}}


&nbsp;

## Id Attribute

- Used to **uniquely** identify elements on a page

- No two elements should have the same id value (otherwise it would not be unique)

```
  <!-- in html -->

  <button id='add-task'> Add Task </button>

```

```
  // in css a '#' (hash) is used to specify an id selector 

  #add-task {
    font-size: 12px;
  }


```

{{% notice tip %}}
  In css **id** selectors are specified using a ``#`` (hash)
{{% /notice %}}


&nbsp;

## Naming classes and ids

- Developers can choose any name they want for classes and ids, however the names you choose should be descriptive


&nbsp;

## When should you use classes instead of ids (or vice versa)?

- Use classes if applying a general style to more than one element on the same page

- Use ids when you style element differently from any other instance of the same element

- Use ids when using javascript to precisely target elements



