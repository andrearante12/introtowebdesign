[BACK TO FULL COURSE DESCRIPTION](https://github.com/Andre-Arante/introtowebdesign)

# Week 7 - Transitions

# State Changes

Types of stage changes

- moving mouse over link (or any other type of element)
- change in window size
- scrolling causes elements to disappear (or appear)

## `a:hover { ... }` - psuedo class

- allows you to make conditional declarations after certain user interactions
- e.g. :focus, :visited, :disabled, :active

# Duration

Two parts:

- property that we want to transition
- duration

Example:

    a {
    transition-property: color;
    transition-duration: 1s;
    }

When the color is changed, it will <em>blend</em> into the new color over a period of 1s.

`color` can be replaced by a sizing property such `font-size`, `width`, or `height`. This will result in the element growing/shrinking.

400ms, or the speed a human blinks at is typically a good duration.

# Timing Function

    transiton-timing-function: ease;

By default, transitions will start slow, speed up, and end slow

Other options include:

- `ease-in` — starts slow, accelerates quickly, stops abruptly
- `ease-out` — begins abruptly, slows down, and ends slowly
- `ease-in-out` — starts slow, gets fast in the middle, and ends slowly
- `linear` — constant speed throughout

If interested... <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function">full list of options</a>

# Delay

Specifies the amount of time to wait before a transition starts

    transition-delay: 400ms;

Again, 400ms is the conventional time.

# Shorthand

    transition-property: color;
    transition-duration: 1.5s;
    transition-timing-function: linear;
    transition-delay: 0.5s;

can be expressed as

    transition: color 1.5s linear 0.5s;

Using this shorthand, you can also chain commands together to create more complex animations

    transition: color 1s linear,
    font-size 750ms ease-in 100ms;

It is possible to simplify even more using the `all` keyword. With this, all properties that change will have the same effect applied to them.

    transition: all 1.5s linear 0.5s;
