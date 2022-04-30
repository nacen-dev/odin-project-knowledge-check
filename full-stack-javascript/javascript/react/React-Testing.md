# React Testing

## Knowledge Check

### What packages are required for React testing?

- @testing-library/react
- @testing-library/jest-dom which is optional
- @testing-library/user-event

### What is the significance of the user-event package?

It simulates user interactions with the webpage.

### What does the render method do?

The `render` method renders a React.element to a container which is appended to document.body

### What is the most preferred method for querying?

`getByRole` as it ensures that the UI is accessible as it can query every element exposed in the accesibility tree

### How would you test for a click event with userEvent?

Using the click function of userEvent

`userEvent.click()`

### What is the advantage of snapshot tests?

- Fast and easy to write

### What are the disadvantages of snapshot tests?

- False negatives as changes easily break the snapshot tests
- False positives as it cannot ascertain validity of a component, bugs might go undetected.

### How can you mock a callback handler?

Using jest we can mock functions using jest.fn()

### How can you mock a child component?

Using jest.mock and only rendering bare minimum to realize the validity of the component