# Advanced Grid Properties

## Knowledge Check

### How do you create several grid tracks of the same size without manually typing each one out?

Using the `repeat` function

### What is the difference between a static and dynamic size value?

A static value does not change, while a dynamic size value is flexible can change depending on context when it reaches a certain condition

### How can you assign a grid track a flexible value that changes depending on the remaining space available in the grid?

Using fractional units which is the `fr` unit

### How can you assign grid tracks an uneven distribution of the remaining space in a grid?

You can use the fr unit to use the fractional space 1fr will cover the 1 fractional unit 2fr will take up to 2 fractional units of the remaining space in the grid.

### Which CSS functions will return the smallest or largest value supplied to them?

- `min` returns the smallest value
- `max` returns the largest value

### Which CSS Grid-only function allows you to supply a minimum and maximum track size that is calculated in realtime?

`minmax` function

### Which global CSS function allows you to supply a minimum, ideal, and maximum value that is calculated in realtime?

`clamp` function

### What attribute of repeat() can be used to fill in as many grid tracks as possible, given certain constraints?

auto-fit and auto-fill

### What is the difference between auto-fit and auto-fill?

- `auto-fit` fills all available space and collapses the next row/column if there is no content and then expand the grid items

- `auto-fill` on the other hand will fill the row/column but does not expand the grid items even if there is no content that is occupying the next row/column 
