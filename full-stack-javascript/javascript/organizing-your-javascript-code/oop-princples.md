# OOP Principles

## Knowledge Check

### Explain the “Single Responsibility Principle”.

The Single Responsibility Principle states that a class/object should only have one responsibility, that it should do that responsibility well and only that responsibility.

An example would be

```
const add = (x, y) => {
  let sum = x + y;
  console.log(sum);
}
```

In this simple example the add function is doing two responsibility it's doing the logic of adding two numbers and also the logic for logging it to the console, in which it should not do. It should only do one responsibility which is to add the two functions.

This second example now follows the Single Responsibility Principle

```
const add = (x, y) => {
  return x + y;
}

```


### Briefly explain the additional SOLID principles.

#### Open Closed Principle

Objects should be open for extension but closed for modification, which means that object can be changed through extension where it depends on the method for extending it but the object cannot be modified directly.

#### Liskov Substitution Principle

A class that inherit from it's parent can be a substitute to it's parent. 

Let's say we use the subclass on a function that expects the parent class that should not break our program since the subclass inherit from it's parent there should be no issue using it as a substitute. 

#### Interface Segregation Principle

Interface Segregation Principle states that the client that implements the interface should not be forced to implement an interface that it doesn't use or depend on method that it does not use. So our interface should only contain what should be implemented.

#### Dependency Inversion Principle

Object must depend on abstractions not on concretions. In JavaScript this pattern is easily followed by using a higher order function.

### Explain what “tightly coupled” objects are and why we want to avoid them.

Tightly coupled objects are objects that knows, or is dependent on another object, the reason we want to avoid them is that tightly coupled objects can easily break when one object changes in which we need to also change the object that depends on the object that changed. This reduces re-usability and flexibility in our code.