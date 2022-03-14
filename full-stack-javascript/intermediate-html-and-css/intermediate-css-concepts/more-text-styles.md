# More Text Styles

## Knowledge Check

### What are the 2 ways to add fonts that are not installed on a user’s computer?

1. Using the link tag

Example
```
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet"> 
```
2. Using the @import tag inside your css, preferably at the top

Example
```
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
```
### What is the ‘system font stack’ and why would you want to use it?

The system font stack is a series of fonts, it is used if the font you specified is not installed on the system it then goes through this stack of fonts until it finds one that is installed on the system

```
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

// It will check if you have the first font if not it will check if you have the second font, and so on and so forth.
```

### Which property would you use to increase or decrease the space between letters in a word?

letter-spacing

### Which property would you use to increase or decrease the space between lines in a paragraph?

line-height
