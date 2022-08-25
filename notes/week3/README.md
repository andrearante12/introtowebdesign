[BACK TO FULL COURSE DESCRIPTION](https://github.com/Andre-Arante/introtowebdesign)

# Week 3 - Typography

- [Font Families](#font-families)
- [Font Weight](#font-weight)
- [Font Style](#font-style)
- [Text Transform](#text-transform)
- [Text Layout](#text-layout)
- [Text Alignment](#text-alignment)

"The art of arranging text on a page"

We use fonts and positioning to achieve good typography.

# Font Families

<a href="https://www.cssfontstack.com/">Web Safe Fonts</a>

```
h1 {
  font-family: Caslon, Georgia, 'Times New Roman', serif;
}
```

<img src="https://content.codecademy.com/courses/web-101/htmlcss1-diagram__fontanatomy.svg">

serif - more old fashioned

sans-serif - more modern looking

# Font Weight

<p style="font-weight: bold;">bold</p>
<p style="font-weight: normal;">normal</p>

Numerical options: 1(lightest) to 1000(boldest)

# Web Fonts

https://fonts.google.com/

# Text Transform

`text-transform: uppercase || lowercase`

# Text Layout using `letter-spacing` and `word-spacing`

`letter-spacing: 2px;`

<p>No Spacing</p>
<p style="letter-spacing: 10px;">10px Spacing</p>

<br>

<p>No Word Spacing</p>
<p style="word-spacing: 10px;">10px Word Spacing</p>

# Text Alignment using `text-align`

<p style="text-align: right;">Right</p>
<p style="text-align: left;">Left</p>
<p style="text-align: center;">Center</p>

# Positioning

By default elements take up the full width of their container.

This property can be changed by using a declaration to the `position` property.

By default: `position: static;`

# Relative

Allows you to <em>offset</em> the element from its default position.

- `top` - moves the element down from the top.
- `bottom` - moves the element up from the bottom.
- `left` - moves the element away from the left side (to the right).
- `right` - moves the element away from the right side (to the left).

```
.green-box {
  background-color: green;
  position: relative;
  top: 50px;
  left: 120px;
}
```

# Absolute

All other elements on the page will ignore this element. This allows you to have overlapping elements.

# Fixed

An element with a fixed position will remain in that position even if the user scrolls

# Sticky

Similar to fixed, but allows for the element to be "scrollable" until it reaches a certain position, at whichpoint it will become "stuck."

# Z-Index

Ordering for elements that overlap.

Important things to note:

- does not work with `static` elements
- default z-value is 0
- a z-value of 1 will move an element forwards

This is also used with navbars
