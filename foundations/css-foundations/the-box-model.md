# The Box Model

## Knowledge Check

### From inside to outside, what is the order of box-model properties?

1. Content Box
2. Padding Box
3. Border Box
4. Margin Box
   <br />
   <br />

### What does the box-sizing CSS property do?

- It sets how the total width and height of an element is calculated.
  <br />
  <br />

### What is the difference between the standard and alternative box model?

- The standard is set to content box, any border or padding will be added to the final rendered width, and height.

  ```
  div {
    width: 100px
    margin: 20px;
  }
  ```

  total width = 120px;

- The alternative box model accounts the border and padding to the final width and height rendered by the element in which the content will shrink or expand to the available space left after the calculation .
  ```
  div {
    box-sizing: border-box;
    width: 100px;
    padding: 20px;
    border: 5px solid black
  }
  ```
  This will set the width to 100px with a padding of 20px on all sides you will only have 50px for the content. content = width 100px - padding 20px*2 - border 5px*2 as it's on bothsides = 50px
  The total width is still 100px.
  <br />
  <br />

### Would you use margin or padding to create more space between 2 elements?

- I would use the margin to create more space between 2 elements
  <br />
  <br />

### Would you use margin or padding to create more space between the contents of an element and its border?

- I would use padding to create more space between the contents of an element and it's border
  <br />
  <br />

### Would you use margin or padding if you wanted two elements to overlap each other?

- I would use margin to overlap two elements with each other.
