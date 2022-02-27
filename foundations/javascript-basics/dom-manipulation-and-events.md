# Dom Manipulation and Events

## Knowledge Check

<br />

### What is the DOM?

The DOM (Document Object Model) is a tree like representation of a web page.

### How do you target the nodes you want to work with?

You target the node you want by using selectors similar to CSS

Example

```
const container = document.querySelector("#container"); // selects an element that has an id of container
```

### How do you create an element in the DOM?

Using the document.createElement creates a new element into the DOM but does not add it yet.

```
const div = document.createElement('div');
```

### How do you add an element to the DOM?

You add an element to the node by selecting the parentNode and either using the appendChild or insertBefore method

```
parentNode.appendChild(childNode) appends childNode as the last child of parentNode
parentNode.insertBefore(newNode, referenceNode) inserts newNode into parentNode before referenceNode

const newDiv = document.createElement('div'); // creating an element

const container = document.querySelector("#container"); // selecting the element with an id of container

container.appendChild(newDiv) // appending the newDiv as the last child of container

```

### How do you remove an element from the DOM?

Using the removeChild method from the parentNode

```
parentNode.removeChild(child)
```

### How can you alter an element in the DOM?

You can alter an element in the DOM by selecting the element and from there it will give you property and methods you can use to change an element

```
const container = document.querySelector("#container");

container.style.color = "green";

```

### When adding text to a DOM element, should you use textContent or innerHTML? Why?

It is better to use textContent as innerHTML can be used for a Cross Site Scripting Attack

### Where should you include your JavaScript tag in your HTML file when working with DOM nodes?

To include the javascript tag at the bottom of the HTML file so the nodes will be created first before the javascript code is run.

Alternatively we can use the defer attribute inside the script tag which loads the file after the HTML is parsed and ready.

```
<script src="index.js" defer></script>
```

### How do “events” and “listeners” work?

Events are actions that happened on the webpage, while listeners will check if a certain event happened so it will run a function that you give

```
btn.addEventListener("click", () => console.log("button clicked")); // add an event listener to the button to check if was clicked, if it was clicked it will run the function
```

### What are three ways to use events in your code?

1. Adding events inline in the html tag

2. Adding a selector to the element and creating a separate javascript file to add the event to the selected element

3. Using Event Listeners

### Why are event listeners the preferred way to handle events?

Because it is more flexible and powerful since we can add more listeners if the need ever arises.

### What are the benefits of using named functions in your listeners?

The benefits of using a named function in your listeners is that you can reuse it and the name can be used to identify what the function does 

### How do you attach listeners to groups of nodes?

We first need to select the group of nodes and then loop over the group of nodes. lastly we attach the event listener to each node

```
// html file

<div id="container>
  <p class="text">...</p>
  <p class="text">...</p>
  <p class="text">...</p>
</div>

// js file

const paragraphs = document.querySelectorAll(".text");
paragraphs.forEach((paragraph) => {
  paragraph.addEventListener("focus", () => {
    paragraph.backgroundColor = "#001219"
    paragraph.color = "#e9d8a6"
  })
})
```

### What is the difference between the return values of querySelector and querySelectorAll?

- querySelector returns a reference to the first match of the selector 

- querySelectorAll returns a nodelist containing reference to all of the matches of the selector

### What does a “nodelist” contain?

A nodelist contains the reference to all of the matches of the selector it looks very similar to an array but it is not an array.

### Explain the difference between “capture” and “bubbling”.

Capture refers to capturing an event that happened inside an element by traversing down to the target element while bubbling refers to an event that happened inside one element bubbling up to it's parent up to other ancestors.