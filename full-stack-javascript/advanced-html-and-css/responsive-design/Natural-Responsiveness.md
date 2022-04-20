# Natural Responsiveness

## Knowledge Check

### Why should you avoid fixed width?

Because a fixed width won't shrink on a lower screen size which will result into an overflow

### Why should you avoid fixed height?

Similar to avoiding a fixed width it will result into an overflow

### In what situations might it be appropriate to use a fixed height or width?

A example given would be icons or sidebars where it is appropriate to use fixed height or width.

### Why should you avoid percentages?

The reason stated in this [article avoiding percentages](https://codyloyd.com/2021/percentages/) I read is that most elements are already responsive on to the viewport, even without using percentages. According to the article this leads to less than aesthetically pleasing combinations. The article suggest not using a percentage, but rather leaving the element as it is or if you do not want the element to occupy the full width is to use static padding and margin in the element and having a static max-width.