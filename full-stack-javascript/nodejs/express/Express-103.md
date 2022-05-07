# Express 103 Routes and Controllers

## Knowledge Check

### How do you define a route function in Express?

```
const express = require('express');
const router = express.Router();

router.get("/", (req, res) => {

})

```

You define it by adding a http verb after router. then that function will take in a path and a function to handle that pattern

### Name four HTTP verbs a route might need to handle.

- GET
- POST
- PUT
- DELETE

### What is a route parameter, and what syntax is used to define one in a route handler?

Route parameters are named URL segments used to capture values at specific positions in the URL. The named segments are prefixed with a colon and then the name (e.g. /:your_parameter_name/. The captured values are stored in the req.params object using the parameter names as keys (e.g. req.params.your_parameter_name).

### What is a route-handler callback function commonly called?

Controller modules