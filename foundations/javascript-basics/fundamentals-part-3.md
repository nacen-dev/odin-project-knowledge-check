# Fundamentals Part 3

## Knowledge Check

### What are functions useful for?

Functions are useful for not repeating code in your program, as it allows you to contain a piece of code in the program and easily run it by invoking the function without having to copy and paste it again and again in the program.

### How do you invoke a function?

You invoke a function by adding () after the function name

```
console.log // function
console.log() // invoking a function
```

### What are anonymous functions?

Anonymous functions are functions that doesn't have a name associated with them, often used on another function that expects to receive another function as a paremeter.

### What is function scope?

Function scope refers to code inside a function where they are considered as a separate environment. The code inside are contained and are unreachable from the code outside the function.

### What are return values?

Return values are the values that a function has returned after its completion.

### What are arrow functions?

Arrow functions are another way to create function using the arrow syntax which translates to function takes this input and produces this ouput on the right of the arrow.

```
const getAge = age => console.log(`Your age is ${age}`)
```