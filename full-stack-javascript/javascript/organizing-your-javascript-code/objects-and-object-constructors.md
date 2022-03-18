# Objects and Object Constructors

## Knowledge Check

### Write an object constructor and instantiate the object.

```
function Book(name, author, pages, read) {
  this.name = name;
  this.author = author;
  this.pages = pages;
  this.read = read;
}

const FirstBook = new Book("Atomic Habits", "James Clear", 300, true)
```

### Describe what a prototype is and how it can be used.

A prototype is another object that the current object inherits from.

```
function Book(name, author, pages, read) {
  this.name = name;
  this.author = author;
  this.pages = pages;
  this.read = read;
}

Book.prototype.info = function () {
  console.log(`Book Name: ${this.name}, Author: ${this.author}, Pages: ${this.pages}, Read: ${this.read ? "read" : "not read yet"}`)
}
```

We can use it to declare methods that can be shared on all instances of the Object instead creating new set of functions each time it's instantiated which increases memory usage, we can use the prototype so this function is shared in all object that inherits from the prototype.

### Explain prototypal inheritance.

Prototypal inheritance is a feature that helps object inherit methods and properties of another object, it can be done by setting the object prototype to another object that it wants to inherit methods and properties from.

### Understand the basic do’s and don’t’s of prototypical inheritance.

#### Do

Use Object.create to set the prototype of an Object

#### Don't

Directly setting one's object prototype from another object prototype


### Explain what Object.create does

It creates a new object, using an existing object as the prototype of the newly create object.
