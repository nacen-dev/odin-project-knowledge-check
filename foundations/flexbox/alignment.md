# Alignment

## Knowledge Check

### What is the difference between justify-content and align-items?

- Justify content aligns the children of the flex container within the main axis, while the align items property aligns the children within the cross axis

### How do you use flexbox to completely center a div inside a flex container?

- You use both justify content and align-items to completely center a div inside a flex container

```
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```


### What’s the difference between justify-content: space-between and justify-content: space-around?

- The difference between the two is that space-between gives space between the elements so it gives space on the middle, but on space around it also gives space on the left and right of the element 

A simplified overview of the difference is shown below
```
justify-content: space-between: element *space * element
justify-content: space-around: *space* element *space* element *space*
```