# More Testing

## Knowledge Check

### What is tightly coupled code?

A tightly coupled code means that the code depends on another code outside of its own code.

### What are the two requirements for a function to be pure?

1. The function always return the same result if the same argument are passed into the function. It must only depend on it's input arguments.

2. The function does not produce side effects(mutation, network request and etc)

### What are side effects and why is it important to identify them when testing a function?

Side effects is when a function relies on or modifies, something outside it's parameters to do something.

### What are two solutions to the tightly coupled code problem?

1. Remove the dependencies from the code.
2. Mocking

### What is mocking?

Writing fake versions of a function that always behaves exactly how you want.

### When would you use a mock function?

For function that produces side effects like a network request, we don't want to call the network request when testing as it will slow down the test execution, we can use a mock function instead.

### How should you test incoming query messages?

Making assertions about what they send back

### Why should you not test implementation?

Because implementation of the code can change, what must be tested is the interface.

Also according to Kent C. Dodds

1. Test can break when you refactor your code. False negatives
2. Test may not fail when you break your code. False positives

### Should you test private methods?

The rule was not to test private methods as it's an anti-pattern.

- Do not make assertions about their result
- DO not expect to send them

### Why should you not test messages with no side effects?
