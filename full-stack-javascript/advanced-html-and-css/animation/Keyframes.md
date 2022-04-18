# Keyframes

## Knowledge Check

### What are the long and short-hand notations for CSS animations?

#### Long notation

animation-name, animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, animation-fill-mode, and animation-play-state

##### Short-hand

/* @keyframes duration | easing-function | delay |
iteration-count | direction | fill-mode | play-state | name */

animation: 3s ease-in 1s 2 reverse both paused slidein;

### How do you add keyframes to an animation?

```
@keyframes <animation-name> {

}
```

### When would you use an animation over a transition (and vice versa)?

- Looping
- If animation does not need a trigger
- Flexibility
