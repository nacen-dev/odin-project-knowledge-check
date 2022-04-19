# Keyboard Navigation

## Knowledge Check

### What are two things that interactive elements must have for keyboard users?

1. Focus Styles
2. Tab Order

### What are focus styles?

Focus styles refers to the styles applied when an element is focused, by default interactive elements have focused styles set.


### Why should you never completely remove focus styles from an element?

Focus styles helps the user as it provides visual indication if an element is focused or not, by removing it we won't know if a certain element is focused

### What is the tab order?

The tab order is the order in which element will receive focus when you press the `Tab` key, by default it will have the same order as it's listed in the html.

There are times when the tab order is different from the visual order, to solve this it would be better to structure your content on the markup as the order that is needed, or correct it by placing the correct tabindex into the element

### What is the best way to hide hidden content from assistive technologies?

Using either `display: none`, or `visibility: hidden` to also hide the content not just visually from the screen but also from assistive technologies. 