+++
toc = true
prev = "/02-css-basics/html-review-exercise"
next = "/02-css-basics/css-intro"
weight = 11
title = "Relative Paths"
date = "2017-01-22T18:08:00-05:00"

+++

## Relative Paths

- Relative URLs can be used when linking to pages and files **within your own website**.

- Shorthand way of telling the browser where to find your files.

- Inform students that they have already seen this is use with the link tag when referencing a css file

----

## Example Project with Multiple Folders/Files

![This is an image](/images/02/folder_structure_image.png)


## Navigating within the Same Folder

Linking from **music index** page to the **music reviews** page

```
<a href="reviews.html"> Music Reviews </a>

```

----

### Navigating to a file in a Child Folder

Linking from the **homepage (top-level index.html)** to the **music listings** page

```
<a href="music/listings.html"> Music Listings </a>

```

----

### Navigating to a file in a Grandchild Folder

Linking from the **homepage (top-level index.html)** to the **dvd reviews** page

```
<a href="movies/dvds/reviews.html"> DVD Reviews </a>

```

----

### Navigating up to a file in a Parent Folder

Linking from the **music reviews** page to the **homepage (top-level index.html)**

```
<a href="../index.html"> Home </a>

```

Use `../` to move up **exactly 1 level** in the folder hierarchy

----

### Navigating up to a file in a Grandparent Folder

Linking from the **dvd reviews** page to the **homepage (top-level index.html)**

```
<a href="../../index.html"> Home </a>

```

Here we used `../../` to move up 2 levels in the folder hierarchy
