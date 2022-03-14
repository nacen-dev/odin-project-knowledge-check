# Form Validation

## Introduction

Validations allow us to set specific constraints or rules that determine what data users can enter into an input. When a user enters data that breaks the rules, a message will appear, providing feedback on what was wrong with the entered data and how to fix it.

Validations are a vital ingredient in well-designed forms. They help protect our backend systems from receiving incorrect data, and they help make the experience of interacting with our form as dead-stupid-simple as possible for our users.

## Knowledge Check

### What does the required validation do?

It prevents the user from submitting the form when the form control that has a required attribute has an empty value

### What validations can you use for checking text length?

```
<input type="text" minlength="3" maxlength="20" />
```

### How can you validate the minimum and maximum of numeric inputs?

```
<input type="number" min="1" max="10" />
```

### What can you use the pattern validation for?

You can use the pattern validation for a lot of things to get the correct input from a user, for example we could use it for checking address, phone number, credit card number if it's in the correct format.

### What pseudo css selectors are available for styling valid and invalid inputs?

- :valid 

- :invalid