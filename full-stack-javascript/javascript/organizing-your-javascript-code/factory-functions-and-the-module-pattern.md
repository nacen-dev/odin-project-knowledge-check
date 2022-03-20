# Factory Functions and the Module Pattern

## Knowledge Check

### Describe common bugs you might run into using constructors.

- Forgetting the `new` keyword and polluting the global namespace as a result

### Write a factory method that returns an object.

```
const bookFactory = (name, author) => {
  const info = () => console.log(`Book Name: ${name}, Author: ${author}`);

  return {
    name,
    author,
    info
  }
}
```

### Explain how scope works in JavaScript (bonus points if you can point out what ES6 changed!).

Scope is the current context of the code on Javascript. What are the current available data(variable) I have access to right now.

We can think of it of a circle inside another circle. Anything that is in the outer circle can be accessed by the inner circle, but anything inside the inner circle cannot be accessed by the outer circle.

ES6 introduced let and const which gives block scope this means that this variable will only be accessible inside the block where it was set, it cannot be accessed outside of that block. Block refers to a set curly bracket

```
let a = 5; // global scope

if (a >= 3) { <-
  let b = a + 5; // block scope
  if (b > 10) {
    console.log(b) // b is only accessible right now to the block where it was declared
  }
-> }

console.log(b) // reference error since b is only accessible inside the block where it was declared.
```

### Explain what Closure is and how it impacts private functions & variables.

Closure is a concept where a function having access to their scope even after the parent function has finished executing.

Closure allows us to create private function and variables since Closure still retains access to the variable and function of it's parent function in which we can create methods inside the closure that can access the variable and function of it's parent and only expose what is needed, in this case it creates private functions and variables since it cannot be accessed outside.

### Describe how private functions & variables are useful.

Private functions and variables are useful because data is protected from being accessed outside, which can potentially avoid accidental assignment, re-assignment

### Use inheritance in objects using the factory pattern.

```
const Book = (name, author) => {
  const info = () => console.log(`Book Name: ${name}, Author: ${author}`);

  return {
    name,
    author,
    info
  }
}

const HistoryBook = (name, author) => {
  const { info } = Book(name, author);
  const type = "history";

  return {
    type,
    info
  }
}

const historyBook1 = HistoryBook("AP 1", "Author");
historyBook1.info();

```

### Explain the module pattern.

A module is similar to a factory function, but it's created through an `IIFE` instead. It's a pattern used to create a single instance of the object and you can reveal only what is needed since it uses closure.

### Describe IIFE. What does it stand for?

IIFE is a function that is immediately executed. It stands for Immediately Invoked Function Expression.

### Briefly explain namespacing and how it’s useful.

Namespacing is a technique to avoid naming collision. It's useful as functions could have the same name from another script or library in which can gives you errors with namespacing the function is encapsulated inside of the object book.info(), person.info() and etc.
