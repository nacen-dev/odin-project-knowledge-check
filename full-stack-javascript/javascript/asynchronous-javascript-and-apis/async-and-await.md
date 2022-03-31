# Async and Await

## Knowledge Check

### How do you declare an async function?

Adding async keyword in the function an example is shown below.

```
async function myFunction() {

}

const arrowFunc = async () => {

}
```

### What does the async keyword do?

The async keyword makes the function return a promise.

### What does the await keyword do?

The await keyword as it name suggest waits for the promise to be resolved, then it either throws an error if an exception is generated or it returns the result.

### What is returned from an async function?

What is returned from an async function is a Promise.

### What happens when an error is thrown inside an async function?

The control jumps to a catch block, but if there is no catch block inside the async function, then you can append a .catch to handle the error, if there is no .catch to handle it as well then you would get a unhandled promise error.

### How can you handle errors inside an async function?

Using a try catch block inside an async function or chaining a .catch to the async function.