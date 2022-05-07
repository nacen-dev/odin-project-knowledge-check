# Express 104

## Knowledge Check

### Why do we use the async module?

We use the async module because most operations in Node are asynchronous, the async module helps us by providing methods to handle the async operation flow based on what we need without experiencing callback hell




### Why are async methods needed and what do they avoid?

The async methods are needed because they provide a better and efficient approach in handling asynchronous operation specifically if you need to make multiple it's better to run them in parallel because if not it will be inefficient and you might have to implement and experience callback hell.

### How do we run multiple asynchronous operations in parallel?

- Using the async.parallel() to execute any operations that must be performed in parallel.


### How do we run multiple asynchronous operations in series?

- Using the async.series() for when we need to ensure that asynchronous operations are performed in series.


### When do we use async.waterfall() instead of async.series() ?

If the asynchronous operation is dependent on the result of the previous operation.

### How do we nest elements and define attributes in Pug?

Elements that are nested are indented and attributes are defined in parentheses after their associated element

### What is a base template and how do we extend it?

A base template is a template that can be extended so other view template use it instead of having to redefine the boilerplate code for html structure.

We extend it by using the extend keyword

```
extends layout

block content
```

### Why do we use luxon instead of the regular date format?

Because the regular date format looks ugly, luxon is a library that can parse, validate, manipulate, format, and localize dates.

