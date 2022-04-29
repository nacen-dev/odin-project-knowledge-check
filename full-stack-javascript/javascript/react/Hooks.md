# Hooks

## Knowledge Check

### How do you declare state in a functional component?

Using the useState hook

```
const [state, setState] = useState(initialValue);
```

### What is the correct naming convention for state values?

To use the second value like the first value, but prefixing it with a set

```
const [todo, setTodo] = useState()
```

### How do you mimic componentDidMount, componentDidUpdate and componentWillUnmount in a functional component?

Using the useEffect hook

```
useEffect(() => {

  return () => { // cleanup function

  }
}, [dependency]) // dependency array is equivalent to componentDidUpdate or if without any dependency it is equivalent to componentDidUpdate
```

### Explain how the dependency array in the useEffect hook impacts the effect of the hook?

If a dependency is specified the useEffect hook will run each time the dependency changes, if the depdency array is empty the useEffect will only run on it's initiall render.