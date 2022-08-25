[BACK TO FULL COURSE DESCRIPTION](https://github.com/Andre-Arante/introtowebdesign)

# Week 5 - Responsive Design and the Grid Layout

# Min/Max Values

- min-width
- min-height

If the minimum value is too low, it is possible for elements to spill out. (This is poor design)

## Difference between `height` and `min-height`

`Height` is a <b>fixed</b> value. Setting a `min-height` allows the element to grow/shrink as the page changes

Also worth noting that `min-heigh`t always takes priority.

# Overflow

An element's size comprises of the content, padding, margin, and border all added together.

\*refer to demonstration

The `overflow` property describes what happens to content that is larger than its container

The most common values are:

- `hidden` - hides excess content
- `scroll` - automatically adds a scroll bar
- `visible` - content is shown outside the container (default value)

# Responsive Design

The ability for a website to resize and reorganize content based on:

- size of other content
- size of the screen

So far we have been using pixels, but this is actually bad because we are <em>hard coding</em> values. We want our websites to be reactive.

# Em

Based on the font size of the current element OR the default base font size

In most browsers

- 1 rem = 16px

Useful for when you want to size elements compared to other elements nearby. (e.g. cards)

# Rem

Based on the ROOT element

In most browsers

- 1 rem = 16px

Useful for when you want to size elements consistiently across the whole webpage.

# Percentages

When percentages are used, elements are sized relative to their parent. This means that they will take up a percentage of the total space avaliable within the parent.

Note: It is bad practice to set height/width to 100% because this does not account for margins/padding and may cause components to overflow.

## Note about relative sizing

When using relative sizing, ems and rems should be used to size text and dimensions on the page related to text size (i.e. padding around text). This creates a consistent layout based on text size. Otherwise, percentages should be used.

# Scaling Images/Videos

```
.container {
  width: 50%;
  height: 200px;
  overflow: hidden;
}

.container img {
  max-width: 100%;
  height: auto;
  display: block;
}
```

This is a very common design pattern for this scenario.

`background-size: cover;`
