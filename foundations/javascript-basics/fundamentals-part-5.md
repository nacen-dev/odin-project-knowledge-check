# Fundamentals Part 5

## Knowledge Check

### What is the difference between objects and arrays?

Objects stores data through key value pairs unlike arrays where index is assigned for each element, Objects uses key/property name to access the value

```
// Objects
let user = {
  firstName: "Nacen",
  lastName: "Dev"
}

user.firstName
user["firstName"]

// Arrays
let user = ["Vincent", "Nadal"]
user[0] // Vincent
```

### How do you access object properties?

- Dot notation (.)
- Square bracket notation []

```
let user = {
  firstName: "Vincent",
  lastName: "Nadal"
}

user.firstName // Vincent
user["firstName"] // Vincent
```

### What is Array.prototype.map() useful for?

It is useful when you want to iterate through all the values in an array and modifying each value.

### What is Array.prototype.reduce() useful for?

It is useful when you want to reduce an array into a singular value, most common use case getting the total of all the values from the array.
