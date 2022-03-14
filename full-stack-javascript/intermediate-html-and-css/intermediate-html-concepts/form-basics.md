# Form Basics

## Introduction

Forms are one of the most critical parts of your site. They are your user’s gateway into your backend – the user provides data in a form, and you do stuff with it.

You need to specify the proper types of inputs for each possible data item since there are often multiple ways to collect a piece of data, but only one way is easiest for your user.

## Knowledge Check

### Explain what the form element is for and what two attributes it should always include.

Form element is a container like element similar to a div, where other elements like input tags are nested inside the form element, so every input the user has is wrapped by the form element. 

The two attributes it should always include are the action, and method attribute.

### Explain what form controls are at a high level.

Form controls are the elements the user will interact within the form, such as checkboxes, text box and etc.

### What is the name attribute for?

It is used to serve as a reference to the data inputted into a form control, on the backend it will show up like a variable name for that particular form control.

### What are the three most common form controls you can use for allowing users to select predefined options?

- Select dropdown
- Radio buttons
- Checkboxes

### What are the three types of buttons in html?

- submit 
- reset
- button

the submit type will submit the data inside the form, where it gets sent is based on the action attribute of the form element.

the reset will remove and reset all data inside the form to a clear state.

the button type have no effect so it's mostly used to do a customized behavior of a button by using Javascript

### What are the two most challenging aspects of styling forms?

- Default Browser Styles 
- Tricky and downright impossible to style form controls