+++
title = "Background Images"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/05-css-positioning-and-colors/css-positioning"
next = "/05-css-positioning-and-colors/code-along"
weight = 15

+++

## ``background-image`` Property

- ``background-image`` property allows you to place an image behind any HTML element

- Image can be "behind" the entire page or part of a page

- **By default** a background image will repeat to fill an entire box

```css
  body {
    /* this image will be applied to the entire page */
    background-image: url("images/cool-background-image.gif");
  }

  .hero-section {
    /* this image will be applied to container with a "hero-section" class attribute */
    background-image: url("images/another-cool-background-image.gif");
  }

```
---

## ``background-repeat`` Property

- ``background-repeat`` allows you to control how an background image is repeated

  1. repeat: image is repeated both horizontally and vertically (default behavior)

  2. repeat-x: image is only repeated horizontally

  3. repeat-y: image is only repeated vertically

  4. no-repeat: image is only shown once and not repeated

---

## ``background-position`` Property

![right ](/images/03/background_position.png)

- Used to position an image **when it is not being repeated**

- This property has two values

  1. horizontal position

  2. vertical position

---

## ``background-position`` Property

```css

  body {
    /* this image will be applied to the entire page */
    background-image: url("images/cool-background-image.gif");
    background-repeat: no-repeat;
    background-position: center top;
  }

```

- If you only specify one value, the second value will default to center

- You can also you pixels or percentages

- They will represent the distance from teh top left corner of the window (or the containing box) top left corner is 0% 0%
