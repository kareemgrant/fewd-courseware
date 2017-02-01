+++
title = "CSS Positioning"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/05-css-positioning-and-colors/css-colors"
next = "/05-css-positioning-and-colors/background-images"
weight = 13

+++

## CSS Positioning

---

### Normal Flow

- Default way browser handles block-level elements

- Each block-level element sits on top of the next one

- If width is not specified, element will span the width of its container


![inline](/images/05/normal_flow.png)

<a class="jsbin-embed" href="https://jsbin.com/rakaya/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

---

### Relative Positioning

- Moves element in relation to where it would have been in normal flow

- Uses offset properties (top or bottom and left or right) to indicate how far to move the element from where it would have been in normal flow

- Usually accompanied by box offsets: top, right, bottom, left.

- It will not effect the other elements on the page

^
If you set position: relative; on an element but no other positioning attributes (top, left, bottom or right), it will have no effect on it's positioning at all, it will be exactly as it would be if you left it as position: static; But if you DO give it some other positioning attribute, say, top: 10px;, it will shift it's position 10 pixels DOWN from where it would NORMALLY be


![inline](/images/05/relative_positioning.png)

<a class="jsbin-embed" href="https://jsbin.com/tavotu/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

---

### Absolute Positioning

- This type of positioning takes box out of normal flow and **no longer affects the position of other elements on the page**

- Other elements act is if the element is not longer there

- Box offset properties (top or bottom and left or right) are used to position the element

- Elements positioned absolutely will be positioned relative to the nearest **positioned** element

Remember that these values will be relative to the next parent element with relative (or absolute) positioning. If there is no such parent, it will default all the way back up to the <html> element itself meaning it will be placed relatively to the page itself.


![inline](/images/05/absolute_positioning.png)

<a class="jsbin-embed" href="https://jsbin.com/cesikiq/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

---

### Fixed Positioning

- Positions the element in relation to the browser window (not its containing element)

- Fixed positioned element stays in place even if user scrolls down the page

- Box offset properties (top or bottom and left or right) specify where the element should appear in relation to browser window

- Example demonstrates how one might create a fixed navbar

{{% notice tip %}}
  A fixed position element is **positioned relative to the viewport, or the browser window itself**. The viewport doesn't change when the window is scrolled.
{{% /notice %}}


![inline](/images/05/fixed_positioning.png)

<a class="jsbin-embed" href="https://jsbin.com/liroqe/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

