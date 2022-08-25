[BACK TO FULL COURSE DESCRIPTION](https://github.com/Andre-Arante/introtowebdesign)

# Week 2 - CSS: Selectors and Colors

- [What is CSS?](#what-is-css)
- [Syntax](#syntax)
- [The Type Selector](#the-type-selector)
- [Class Selector](#class-selector)
- [Id Selector](#id-selector)
- [Multiple Selectors](#multiple-selectors)

# What is CSS?

Short for Cascading Style Sheets, CSS is responsible for making boring HTML look pretty.

# Syntax

<img src="./Screenshot 2022-07-16 231250.png" width="300" >

# Selectors

CSS uses declarations to apply styles to the target of the selector. There are many types of selectors.

# The Type selector

We saw this one last week!

```
body {
    text-align: center;
    background-color: white;
}
```

Notice how it is possible to have multiple declarations within the declaration block.

# Class Selector

```
In our HTML
<div class="purple">Make me purple!</div>

In our CSS
.purple {
    color: purple;
}
```

- Are meant to be resued throughout the website

Important: Don't forget the . (dot) before the class name!

# Id Selector

```
#element-id {
  color: pink;
}
```

- Are only meant to be used once
- Overrides the type and class selectors

`#element-id { color: pink; }` - id selector

# Specificity

Type < Class < Id

# Multiple Selectors

```
h1,
.menu {
  font-family: Georgia;
}
```

- As programmers, we want to avoid unneccesary repetition
