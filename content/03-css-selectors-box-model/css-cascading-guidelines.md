+++
title = "CSS Cascading Guidelines"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/03-css-selectors-box-model/css-selectors"
next = "/03-css-selectors-box-model/box-model"
weight = 12

+++


## How CSS Cascades

There are guidelines that will determine which CSS rule takes precendent in the case of a conflict (when 2 or more css rules target the same selector)

- Last Rule

- Specificity

- Important

- Inheritance

&nbsp;

## Last Rule

- When two or more css rules have identical selectors, the latter of the two rules takes precedent


```

// in css

p {
    color: red;
}

p {
    color: green;
}

```

```
<!-- in html -->

<!DOCTYPE html>
<html>
  <head>
    <title>Sample Page</title>
  </head>

  <body>
    <p> Color will be green</p>
  </body>
</html>

```

Here the `<p>` tag wil be green because the last **conflicting** rule took precedent

&nbsp;

## Specificity

- If one selector is more specific than others, then the more specific rule takes precedent

- For example:

  - **h1** is more specific than **\***
  - **p.discount** is more specific than **p**
  - **#city** is more specific than **img.town**

&nbsp;

## !important

- You can override all the above rules by adding a “!important” after any property

- This **should be used sparingly**; excessive use of **!important** can cause confusion within your codebase



```
// in css

#thing {
    color: green;
}


// add the !important option at the end of your declaration;

p {
    color: red !important;
}

```

```
<!-- in html -->

<!DOCTYPE html>
<html>
  <head>
    <title>Sample Page</title>
  </head>

  <body>
    <p id="thing">Will be RED and NOT Green</p>
  </body>
</html>


```

Here we used the **!important** option in CSS to override the **Specificity guideline** that would have had the rule with the selector of `#thing` take precedence under **normal circumstances**


&nbsp;

## Inheritance

- Certain CSS properties such as font-family, font-size, color will be inherited by child properties

- However, properties such as background color or border properties are not inherited

- Click [here](https://www.w3.org/TR/CSS21/propidx.html) to see a full list inherited and non-inherited CSS properties
