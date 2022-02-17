# Fundamentals Part 1

## Knowledge Check

### Name the three ways to declare a variable?

- `var`
- `let`
- `const`

<br />

### Which of the three variable declarations should you avoid and why?

From the three variable declarations var should be avoided as the scope of this variable is globally available which can be overwritten if another variable declaration with the same name is used on another part of the script.

<br />

### What rules should you follow when naming variables?

- The name must only contain letter, digits or the symbols $ and \_
- The first character must not be a digit

<br />

### What should you look out for when using the + operator with numbers and strings?

The + operator will concatenate the string and number together

<br />

### How does the % operator work?

The % operator is used to get the remainder of the two values in the operation 3 % 2 = 1 because 3 divided by 2 has a remainder of 1.

<br />

### Explain the difference between == and ===.

The == is an equality operator that determines if the value are equal but does not care about the type of the value while === is a strict equality operator which determines if both type and values are strictly equal

```
'1' == 1 // true
'1' === 1 // false
```

<br />

### When would you receive a NaN result?

When you are trying to do an arithmetic operation to a non numeric string

<br />

### How do you increment and decrement a number?

You can increment and decrement a number by using the ++ and -- unary operator

```
let a = 5;
a++ // a = 6
a-- // a = 5

```

<br />

### Explain the difference between prefixing and post-fixing increment/decrement operators.

If we would like to use increase/decrease a value and use the new value immediately we use the prefixing increment/decrement operator.

If we would like to increase/decrease a value, but use the old value instead of the increment/decremented value we use the post-fixing increment/decrement operator.

<br />

### What is operator precedence and how is it handled in JS?

An operator precedence is how the operators are executed on an expression on which operator should be executed first.
It is handled by their precedence, javascript has a precedence table which can be accessed on this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence)

<br />

### How do you access developer tools and the console?

By pressing F12 you will be able to access the developer tools and the console is inside the developer tools window.

<br />

### How do you log information to the console?

console.log allows you to log information to the console.

An example would be

```
console.log("Hello World");
```

<br />

### What does unary plus operator do to string representations of integers?

It converts the string representations of integers to a number
