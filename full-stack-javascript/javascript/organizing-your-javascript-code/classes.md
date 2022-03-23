# Classes

## Knowledge Check

### Describe the pros and cons of using classes in JavaScript.

#### Pros

- It's now easier to create one than before since the class keyword was introduced.

#### Cons

- Under the hood classes in JavaScript is not like the classes in other programming languages like Java since it still uses prototype.
- Bad for Functional Programming

### Briefly discuss how JavaScript’s object creation differs from a language like Java or Ruby.

A JavaScript object creation can be created through various ways like factory function, modules, classes, in which the prototype is used but the concept of class itself does not exist unlike programming languages like Java or Ruby.

### Explain the differences between using a class to define a constructor and other prototype methods.

Using a class provides easier way to define a constructor and other prototype methods mimicking how class are created in other programming languages, unlike the previous way of defining it which can be confusing, with classes it introduces the familiarity because it's syntax follows the syntax of classes in other OOP Languages like Java

### Explain what “getters” & “setters” are.

Getters and Setters are methods defined in a class to interact with one of it's class fields, this way we are not directly changing the field but rather using it's getters and setters to get the value and set the value defined by the creator of the class. This makes use of the concept Encapsulation

### Understand what computed names and class fields are.

- Computed names are dynamic names for a class field/method it's called computed names since the name of the property or method is computed when it's compiled. Allowing this kind of syntax

```
class User {

  ['say' + 'Hi']() {
    alert("Hello");
  }

}

new User().sayHi(); // we get sayHi as the name of that method after the we compute it's value on compilation
```

- Class fields is a syntax that allows to add any properties to the object

### Describe function binding.

Functions in JavaScript has a dynamic this, it depends on the context of the call. Which is why we need to bind the `this` keyword so `this` won't be lost.

Solution

1. A wrapper function
2. bind function

### Be able to use inheritance with classes.

Using the `extend` keyword a class can inherit from another class

### Briefly talk about the conflict in JS with functional programming and classes.

There is a notion called "Favor Composition over Inheritance" and with classes favoring Inheritance it opposes that notion since JavaScript functions are first-class citizens in which Functional Programming is about using them to their full-extent.
