# Custom Properties

## Knowledge Check

### How would you declare a custom property with a name of text-color?

```
--text-color
```

### How would you access a custom property with a name of background-color?

```
var(--background-color)
```

### Where would you declare a custom property to have its scope be global and accessible by all other selectors?

Declare it in the root.

```
:root {
  --text-color: #3dd;
}
```

### Where would you declare a custom property so that a user’s theme setting from their OS or browser was taken into account

Declaring it with the prefers-color-scheme media query

prefers-color-scheme accepts either light or dark

```
@media (prefers-color-scheme: dark) {
  // css code
}
```

or 

```
@media (prefers-color-scheme: light) {
  // css code
}
```