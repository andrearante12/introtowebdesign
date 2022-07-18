# Week 3 - Typography

- [Font Families](#font-families)
- [Font Weight](#font-weight)
- [Font Style](#font-style)
- [Text Transform](#text-transform)
- [Text Layout](#text-layout)
- [Text Alignment](#text-alignment)

"The art of arranging text on a page"

We use fonts and arrangemnts to achieve good typography.

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

<p style="font-weight: lighter;">lighter</p>
<p style="font-weight: bolder;">bolder</p>

- lighter and bolder have a 1 weight difference that their parent

Numerical options: 1(lightest) to 1000(boldest)

# Font Style

```
h3 {
  font-style: italic;
}
```

## Web Fonts

https://fonts.google.com/

Remember `<em>` and `<b>`? They actually apply these declarations under the hood!

# Text Transform

`text-transform: uppercase || lowercase`

# Text Layout

<br><br>

`letter-spacing: 2px;`

<p>No Spacing</p>
<p style="letter-spacing: 2px;">2px Spacing</p>
<p style="letter-spacing: 10px;">10px Spacing</p>

<br><br>

`word-spacing: 2px;`

<p>No Word Spacing</p>
<p style="word-spacing: 2px;">2px Word Spacing</p>
<p style="word-spacing: 10px;">10px Word Spacing</p>

# Text Alignment

`text-align: right;`

<p style="text-align: right;">Right</p>
<p style="text-align: left;">Left</p>
<p style="text-align: center;">Center</p>
