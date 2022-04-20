# Lifecycle Methods

## Knowledge Check

### What is a component’s lifecycle?

Sequence of stages an instance of a component goes through in the DOM

### Explain the most important lifecycle methods

#### Render

It handles the rendering of the component into the DOM

#### ComponentDidMount

To check if a component has already mounted into the dom, so we can start initiating an API call

#### ComponentDidUpdate

To check if a component have updated so we can do something with that update

#### ComponentWillUnmount

Last lifecycle method which means the component is at the end of it's life and usually used to remove event listeners, and other cleanup routines.

### Which tasks should be triggered at the various lifecycle stages of a component?

Initiating API call on ComponentDidMount
Do something if the componentupdates using ComponentDidUpdate
Remove event listeners, cleanups during ComponentWillUnmount