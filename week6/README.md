[BACK TO FULL COURSE DESCRIPTION](https://github.com/Andre-Arante/introtowebdesign)

# Week 6 - CSS Flexbox

Is a tool that allows you to easily position elements

# Flex Container

`display: flex;`

By default, elements with `display: flex;` are block-level elements. This means that the container will take up a whole line.

`display: inline-flex`

This changes the container to an inline element, allowing you to have multiple containers side by side.

# Element Positions

By default, elements are moved to the upper left corner of their container. The `justify-content` property is used to overide this feature and align items horizontally

The `align-items` property does the same but vertically.

See index.html for examples of `justify-content`
See index1.html for examples of `align-items`

# Flex grow/shrink

Flex items shrink proportionally when the container is too small.

\*Note: These properties will be set on the ITEM not the CONTAINER (e.g. an element with the declaration `display: flex;` should not have a `flex-grow` declaration as well)

`flex-grow` allows us to specify:

- if items should grow to fill a container
- which items should grow more/less

Items will grow proportionally:

```
.container { display: flex; }
.middle { flex-grow: 1; }
.sides { flex-grow: 2; }
```

In this example, the sides would each grow to be twice as big as the middle. The math to properly divide the container is done under the hood, and the full space avaliable will always be used.

A max-width can be specifed for an element in order to limit its growth

`flex-shrink` follows a similar behavior, but shrinks elements proportionally rather than growing them.

As with `flex-grow`, a min-width/height can be set in order to limit the shrinkage

## Defaults

By default:

- `flex-grow: 0;`
- `flex-shrink: 1;`

This forces elements to shrink when there is not enough space in the container, ensuring that everything fits in the container

# Flex-basis

Slightly more convoluted, but powerful alternative to min/max dimensions.

If a flex grow is set, the flex-basis serves as a minimum-width. The element will start with width flex-basis, but grow if space is avaliable.

If a flex shrink is set, the flex-basis serves as a max-width. The element will start at flex-basis width, and shrink when needed.

# Flex Shorthand

```
flex: 2 2 100px;
```

is short for

    flex-grow: 2;
    flex-shrink: 2;
    flex-basis: 100px;

```

    flex: 2 1; /* flex-grow=2 flex-shrink=1 */
    flex: 2 20px; /* flex-grow=2 flex-basis=20px */

    /* there is no way to set just flex-shrink and flex-basis in one line*/

```

# Flex Wrap

Sometimes, you want flex items to move to the next line, instead of shrinking to fit the container. This results in a container being more dynamic, but taking up more space.

`flex-wrap: ...;`

Possible values:

- `wrap` - child elements of a flex container that don’t fit into a row will move down to the next line
- `wrap-reverse` - same as wrap, but element order is reversed
- `no-wrap` - default value, elements shrink to fit container

# Align Content

Similar to align-items, but for aligning groups (rows) of items vertically, rather than singular items.

See index2.html for examples

# Axis Review

The main axis is used to position flex items with the following properties:

    justify-content
    flex-wrap
    flex-grow
    flex-shrink

The cross axis is used to position flex items with the following properties:

    align-items
    align-content

# Flex Direction

Allows you to easily change between row and column layouts. Useful in the context of reponsive design (more on this when we get to media queries)

See index3.html for examples.

# Flex-flow

Shorthand for `flex-wrap` and `flex-direction`

Unlike `flex` shorthand, this declaration goes inside of the container

    flex-flow: column wrap;
    flex-flow: row nowrap;
    etc...

## Review (from codecademy)

- display: flex changes an element to a block-level container with flex items inside of it.
- display: inline-flex allows multiple flex containers to appear inline with each other.
- justify-content is used to space items along the main axis.
- align-items is used to space items along the cross axis.
- flex-grow is used to specify how much space (and in what proportions) flex items absorb along the main axis.
- flex-shrink is used to specify how much flex items shrink and in what proportions along the main axis.
- flex-basis is used to specify the initial size of an element styled with flex-grow and/or flex-shrink.
- flex is used to specify flex-grow, flex-shrink, and flex-basis in one declaration.
- flex-wrap specifies that elements should shift along the cross axis if the flex container is not large enough.
- align-content is used to space rows along the cross axis.
- flex-direction is used to specify the main and cross axes.
- flex-flow is used to specify flex-wrap and flex-direction in one declaration.
- Flex containers can be nested inside of each other by declaring display: flex or display: inline-flex for children of flex containers.
