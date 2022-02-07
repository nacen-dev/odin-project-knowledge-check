# CSS Foundations

## Knowledge Check

- What are the main differences between external, internal, and inline CSS?

  - The main differences are
    - external css uses an external css file to be linked to the html page to style the elements
    - internal css are written directly inside the html document within the head element by using the style element
    - inline css is used directly on an html element to directly style it
      <br />
      <br />

- What is the syntax for class and ID selectors?

  - Class selectors `.class, .name` it uses the `.` character to denote it's a class selector
  - ID selectors `#id, #name` it uses the `#` character to denote it's an id selector
    <br />
    <br />

- How would you apply a single rule to two different selectors?

  - You can apply a single rule to two different selectors by selecting them both and adding a comma.

  - An example would be
    ```
    html, body {
      height: 100%;
    }
    ```
    <br />
    <br />

- Given an element that has an id of title and a class of primary, how would you use both attributes for a single rule?
  I would use it like the following syntax below.
  ```
  #title, .primary {
    font-size: 32px;
  }
  ```
  <br />
  <br />
- What does the descendant combinator do?

  - The descendant combinator allows you to select the last element only if it's a descendant of the first selector, an example would be

    ```
    section div {
      width: 100%;
    }
    ```

    We are selecting all divs that are descendants of the section element and then applying the style width 100%

  <br />
  <br />

- Between a rule that uses one class selector and a rule that uses three type selectors, which rule has the higher specificity?
  - The class selector has a higher specificity even if there is a rule that uses three type selectors.
