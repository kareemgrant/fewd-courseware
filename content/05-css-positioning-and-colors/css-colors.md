+++
title = "CSS Colors"
date = "2017-01-22T18:05:18-05:00"
toc = true
prev = "/05-css-positioning-and-colors/code-along-1"
next = "/05-css-positioning-and-colors/css-positioning"
weight = 11

+++

## Specifying Colors in CSS

Several ways to express colors in CSS

- Color Names
- Hex Codes
- RGB, RGBa
- HSL, HSLa

---

## Color Names

- colors represented by predefined names
- 147 color names
- this approach is limited

```css

h1 {
  color: green
}

```

---

## Hex Codes

- colors represented by values for red, green and blue in hexadecimal code

```css

h1 {
  color: #66cdaa
}

```

---

## RGB

- colors represented by values for red, green and blue expressed as numbers between 0 and 255

```css

h1 {
  color: rgb(102, 205, 170)
}

```
---

## RGBa

- Leverages CSS3 inclusion of the **opacity** property
- Just like RGB but allows you to specify the opacity as the fourth value (**alpha** value)
- alpha must be a number between 0.0 and 1.0 (0.5 means 50% opacity)

```css

h1 {
  color: rgba(102, 205, 170, 0.25)
}

```

---

## HSL

- Introduced with CSS3

- Provides an alternative way to express colors based on:

 - Hue (expressed as an angle between 0 and 360 degrees)

 - Saturation (expressed as a percentage)

 - Lightness (expressed as a percentage 0% => white, 50% => normal & 100% => black)


```css

body {
  background-color: hsl(0, 0%, 78%);
}

```
----

## HSLa

- Just like HSL but adds the ability to specify opacity using an **alpha** value

- alpha must be a number between 0.0 and 1.0 (0.5 means 50% opacity)

```css

body {
  background-color: hsla(0, 100%, 75%, 0.5);
}

```
