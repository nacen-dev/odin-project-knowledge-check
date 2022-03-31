# Asynchronous Code

## Knowledge Check

### What is a callback?

A callback is a function that is passed into another function as an argument, which is called by the function that accepts the callback function.

### What is a promise?

A promise is a guarantee that one will do a particular thing or a particular thing will happen.

Mdn's definition of a promise is that the Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.

### When should you use promises over callbacks?

You should use promise over callbacks when you are doing an asynchronous operation.

### What does the .then() function do?

Essentially what the .then() function do is that it will do something with the promise once the promise is resolved. It will either call the onFulfilled or onRejected function (is a call back function that you pass to the then() function), depending on the resolution of the promise.
