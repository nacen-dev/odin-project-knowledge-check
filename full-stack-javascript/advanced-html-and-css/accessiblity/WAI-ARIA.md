# WAI ARIA

## Knowledge Check

### What purpose does WAI-ARIA serve?

To define a way to make web content more accessible when native HTML is unable to do so.

### What are the four things ARIA can’t do?

- modify an element's apperance
- add keyboard event handling
- add focusability
- modify an element's behavior

### What are the five rules of ARIA?

1. Always use native HTML elements and attributes over ARIA when possible.

2. Never change native semantics, unless you have no other choice.

3. All interactive ARIA controls must be usable with a keyboard.

4. Never use role='presentation' or aria-hidden='true' on focusable elements.

5. All interactive elements must have an accessible name

### What is the accessibility tree?

The accessibility is based on the DOM, but the accessibility only contains accessibility related information that will be used by assistive technologies

### What are the differences between the three ARIA labels?

aria-label overrides any native label and modifies the name property in the accessibility tree
aria-labelledby does what aria-label do but it's accessible name is changed to a concatenated string of text or alt attributes of the labeling elements
aria-describedby modifies the description of the element in the accesibility tree

### What does the aria-hidden attribute do?

It hides elements from the accessibility tree, a good example would be using it for decorative images.