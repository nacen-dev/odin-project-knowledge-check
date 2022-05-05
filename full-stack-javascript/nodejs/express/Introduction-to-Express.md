# Introduction to Express

## Knowledge Check

### What is Express?

Express is a Node.js web framework that helps build web server easier than regular node since it it provides mechanisms to:

- Write handlers for requests with different HTTP verbs at different URL paths (routes).
- Integrate with "view" rendering engines in order to generate responses by inserting data into templates.
- Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.
- Add additional request processing "middleware" at any point within the request handling pipeline.

### What is a module?

A module is a javascript library/file you can import or export module for code reuse.

### Which are the four most used methods to define route handlers?

- delete()
- get()
- post()
- put()

### How do we handle errors?

Errors can be handled by one or more special middleware functions that have four arguments (err, req, res, next) but must be called after all other app.use() and routes calls so that they are the last middleware in the request handling process! Express also has a built in error handler which is added at the end of the middleware function stack.

### How do you use the Express library with NPM in a project?

Installing express 
importing the express module
```
const express = require("express");
const app = express();
```
