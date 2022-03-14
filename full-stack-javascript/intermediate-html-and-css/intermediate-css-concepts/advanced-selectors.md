# Advanced Selectors

## Knowledge Check

### What is the difference between the child combinator and the descendant combinator?

A child combinator will only select direct children unlike descendant combinator it will select these element as long as they are a descendant of the parent element so

```
<div>
  <p><p>
  <section>
    <p></p>
  <section>
<div>
```

- `div p` will select all p tag inside the div this is the descendant combinator
- `section > p` will only select p tag that are direct children of a div 

### How does the syntax of pseudo-classes and pseudo-elements differ?

Pseudo classes uses only one `:` colon.

Pseudo elements uses two `::` colon

### Do pseudo-classes exist somewhere in HTML? Do pseudo-elements?

No, they are used to interact with the HTML elements based on their position, structure, state or how the user is interacting with it.

Pseudo elements are used to interact with parts of the HTML that aren't elements at all

### Name two ways you could select every second child of an element, starting with the first.

1. nth-child

2.  nth-type

### What is the difference between div:first-child and div:last-child? What will each select?

### What selector would you use to style a button a user is currently hovering over? How about one that is currently being clicked on?

- button:hover

- button:active

### How could you select all input elements with a type of text?

```
input[text]
```

### How could you select all classes that begin with thunder ?

```
[class^="thunder"]
```