+++
title = "Containing Elements"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/04-page-layout/block-inline-elements"
next = "/04-page-layout/semantic-elements"
weight = 11

+++

## Containing Elements

- Elements that contain groups of elements

- For example, grouping all of the elements associated with the header in a `<div>`

- `<div>` tags are commonly used as containing elements

![inline](/images/04/containing_elements_diagram.png)

In example the above example, orange lines represent `<div>` tags

----

## `<div>`

- Used to group a set of elements together in one block-level box

- `<div>` element are block-level elements which means they will start on a new line


```
<!DOCTYPE html>
<html>
  <head>
    <title>Sample Page</title>
    <link rel="stylesheet" type="text/css" href="css/styles.css">
  </head>

  <body>

    <!-- start of header div -->
    <div id="header">
      <img src="images/logo.gif" alt="Anish Kapoor" />
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="biography.html">Biography</a></li> <li><a href="works.html">Works</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </div>
    <!-- end of header div -->
  </body>
</html>


```

----

## Structure using `<div>`s

- Prior to HTML5, the divs have been the most common way to structure content on page

- Usual ids/classes are used to provide each div with context regarding the type of content div contains

- Above picture is just an example! This structure is not set in stone, use what makes sense for your project

![inline](/images/04/structure_using_divs.png)

{{% notice note %}}
`<div>`s are used to structure pages in logical sections/groups based on your site's layout
{{% /notice %}}


