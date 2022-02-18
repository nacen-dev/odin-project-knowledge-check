# Fundamentals Part 2

## Knowledge Check

### What are the eight data types in JavaScript?

- `number` - for numbers of any kind, integer, floating.
- `bigint` - for big numbers.
- `string` - for characters, zero or more characters.
- `boolean` - true or false.
- `undefined` - default type assigned when no data is assigned to a variable.
- `null` - to explicitly state that the data is null .
- `object` - for creating complex data.
- `symbol` - unique identifier.

<br />

### Which data type is NOT primitive?

Object and Symbols

<br />

### What is the relationship between null and undefined?

Null is when you explicitly state that the data has a null value, while undefined is a default if no data type or value was assigned to a variable

<br />

### What is the difference between single, double, and backtick quotes for strings?

The difference between them is that you will have to escape single quote inside a string that is enclosed with a single quote, which is the same for a string enclosed with a double quote that you will also have to escape double quote characters inside a double quote string

<br />

### What is the term for embedding variables/expressions in a string?

Concatenating

<br />

### Which type of quote lets you embed variables/expressions in a string?

Template literals allow you to embed variables/expressions in a string

<br />

### How do you embed variables/expressions in a string?

By using template literals you can use the $ symbol and enclosed the variables/expression with a { }.

  ```
  let firstName = "Vincent"
  let lastName = "Nadal"
  let fullname = `${firstName} ${lastName}`
  console.log(fullName) // will result to Vincent Nadal
  ```

<br />

### How do you escape characters in a string?

You can escape a characters in a string by using the \ backslash symbol before a certain character or you can use backtick quotes enclosing the strings so you don't have to escape characters.

```
'\'word\'' = 'word'
"\"quotes\"" = "quotes"
`"quote"` = "quotes"
```

<br />

### What is the difference between the slice/substring/substr string methods?

The difference between them is that substring cannot accept negative index, and substr's second parameter takes in the length instead of the position.

<br />

### What are the three logical operators and what do they stand for?

- `&&` the AND operator evaluates both expression and will only return true if both expression evaluates to true else it will return false

- `||` the OR operator evaluates both expression and will return true as long as one of the expression evaluates to true otherwise it reutnrs false

- `^` the NOT operator converts the operand to a boolean

<br />

### What are the comparison operators?

- `>` to compare if the first value is greater than the second value
- `<` to compare if the first value is less than the second value
- `<=` to compare if the first value is less than or equal to the second value
- `>=` to compare if the first value is greater than or equal to the second value
- `==` to compare if the first value is equal to the second value, although it coerce the type and converts the first value to the second if possible which is why it's recommended to use the strict equality operator `===`
- `===` to strictly compare the first value and second value without coercion

<br />

### What are truthy and falsy values?

- In JavaScript truthy and falsy value refers to values that when converted to boolean the value converted will either be false or true,

- A number 0, an empty string "", null, undefined, and NaN all become false. Because of that they are called “falsy” values.

- All other values becomes true

<br />

### What are the falsy values in JavaScript?

- Number 0
- Empty string ""
- null
- undefined
- NaN

<br />

### What are conditionals?

Conditionals are statements used to perform different actions based on different conditions.

<br />

### What is the syntax for an if/else conditional?

```
if (condition) {
  // expression
} else {
  // expression
}
```

<br />

### What is the syntax for a switch statement?

switch() {
  case():
    break;

  default:
    break
}

<br />

### What is the syntax for a ternary operator?

```
condition ? if condition evalueates to true run this code  : else run this code instead
```

<br />

### What is nesting?

Nesting is when you put another expression inside another expression, but if we refer to nesting if statements then it refers to putting another if statement inside an if statement

