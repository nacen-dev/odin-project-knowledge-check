# Transitions

## Knowledge Check

### Are all CSS properties animatable?

No, as not all makes sense to be animated. MDN provides the [list of aminatable properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties)

### What are the long and short-hand notations for transitions?

#### Long notation

```
transition-property: <property> background-color;
transition-duration: <duration> 1s;
transition-timing-function: <timing-function> ease-out;
transition-delay: <delay> 0.25s;
```

#### Short-hand notation

```
transition: <property> <duration> <timing-function> <delay>;
```

### What is the stacking context?

The stacking context is a three-dimensional conceptualization of HTML elements along an imaginary z-axis relative to the user, who is assumed to be facing the viewport or the webpage.

### Why do you need to keep an eye on repaints?

Because CSS transitions can trigger repaint in which you might be repainting not only the element you are animating but also other elements in the stacking context if the element being animated is in the lower stacking context.

The reason being is that whenever the element in the `lower` stacking context was repainted, the browser had to repaint the elements in the `higher` stacking contexts as well.
