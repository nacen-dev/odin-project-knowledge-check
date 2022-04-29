# State and Props

## Knowledge Check

### How do you pass functions, state, or other values between components?

Passing it as a prop

### What is the purpose of state in a React component?

The purpose of state is to track changes in your app, by using state you can do something based on the state.

### Explain the importance of using setState() instead of mutating state directly?

Mutating the state directly might not cause a rerender which is bad because if other components depend on that state they might get incorrect values and not show the correct value

Using setState is the preferred way as it sends a request to update the component after which it will trigger a re-render

### What is the difference between functional and class components and how does their syntax for handling props differ?

Before hooks was introduced functional components were presentational or stateless components and only class components can use state, but with hooks this has changed and right now there is almost no difference except the syntax and some lifecycle methods that the class component has exclusively. Their difference in handling props is as class components it is accessed using this.props but for functional components it can be accessed by the name directly.

### How do you attach event listeners to elements in React components?

Attaching them on synthetic events