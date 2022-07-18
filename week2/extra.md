# IF WE HAVE TIME

- may come back to this during later weeks as these are important

# Chaining

`h1.special { ... }`

- will target only `<h1 class="special">`

# Descendant Combinator

`.main-list li { ... } `

```
IN HTML
<ul class='main-list'>
  <li> ... </li>
  <li> ... </li>
  <li> ... </li>
</ul>
```

- will style all of the `<li>` elements within .main-list

### It is worth noting that more specific selectors (e.g. `li h4 { ... }`) will overide single type selectors (e.g. `h4 {}`)

# Some more advanced selectors

`* { ... }` - universal selector

- this code turns everything pink

- similar to the class selector but will override any other selectors

`img[src*='winter1] { ... }` - attribute selector

- allows you to select based on an element with an attribute

`a:hover { ... }` - psuedo class

- allows you to make conditional declarations after certain user interactions
- e.g. :focus, :visited, :disabled, :active

# Line Height

<p>Default Line</p>
<p>Height</p>

<br>

<p>Line Height</p>
<p style="line-height: 0.2;">of 0.2</p>

<br>

<p>Line Height</p>
<p style="line-height: 5;">of 5</p>
