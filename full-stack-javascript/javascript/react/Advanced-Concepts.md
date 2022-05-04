# Advanced Concepts

## Knowledge Check

### What are PropTypes and why can it be beneficial to use them?

PropTypes as the name suggest gives what type is the prop that the component will receive, if it's a string, number, array, boolean and etc.

### What are Styled Components and how do they make your code cleaner?

Styled Components gives a way to give some default styling to an html element and reusing that throughout your application.

### What is Redux and why are state management systems used in many large applications?

Redux is a state management system where there is a single source of truth for the state of your applications which is stored in the store, this way you don't have to drill your props from one component to another.

### What is prop drilling and how can you use Context API to avoid it?

prop drilling is the concept where you are passing in props to component that doesn't even use them but is needed by one of their child components. Context API provides a way where the parent component can pass the data without having to pass the props to it's child component.

### What is a Higher-order Component?

A Higher order component consumes another component and returns a component. Similar to higher order functions which takes in a function as an argument and returns a function.

### How can you create your own Hooks?

You can create custom hook by composing the available hooks from react like useState, and useEffect in which you call these to a customHook that has a name conventionally that starts with "use"HookName for example a custom hook to load localStorage would be named a useLocalStorage.