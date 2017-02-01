+++
title = "CSS Intro Review"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/03-css-selectors-box-model/agenda"
next = "/03-css-selectors-box-model/classes-and-ids"
weight = 7

+++

## What is CSS?

- Cascading Style Sheet

- Allows you to control design of page

- CSS allows you to create rules that specify how the content of an element should appear


```
p {
  color: black;
}

```

----

## Anatomy of a CSS Rule

![This is an image](/images/02/css_style_anatomy.png)


```

p {
  color: black;
}


h1, h2, h3 {
  font-family: Arial;
  color: #191919;
}


```


----


## Adding CSS to your site

There are three ways to add css to your site

- Inline (avoid!)

- Internal css using `<style>` tag (avoid!)

- External file


----

### Add CSS using an external stylesheet (Recommended/Best Practice)

- The use of external CSS stylesheets allows you to place all of your styles in a central location, any site-wide changes **can be made in a single place**

- A `<link>` tag must be used to connect a stylesheet to an html file


```
<!DOCTYPE html>
<html>
  <head>
    <title>Sample Page</title>
    <link rel="stylesheet" type="text/css" href="css/styles.css">
  </head>

  <body>
    <!-- other tags redacted for example -->
  </body>
</html>


```

```
//in css/styles.css

body {
  font-family: Arial, sans-serif, serif;
  padding: 10px;
}

p {
  font-size: 14px;
  color: #333333;
}



```

----


### `<link>` Tag

- Link tag is used to specify the relationship between an html file and an external file

- Here are some commonly used attributes for the `<link>` tag

  - **href**: specifies the path to the external file

  - **rel**: specifies the relationship between the HTML page and the file it is linked to. The value of this attribute should be stylesheet when linking to a CSS file

  - **type**: specifies the type of document being linked to. This value should be "text/css"


The `rel` attribute is required when linking to css stylesheet

