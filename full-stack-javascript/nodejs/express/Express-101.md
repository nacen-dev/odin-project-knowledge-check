# Express 101

## Knowledge Check

### What is middleware?

A middleware in Express is a function that has access to the request, response object and the next middleware function. 

Middleware functions can perform the following tasks:

Execute any code.
Make changes to the request and the response objects.
End the request-response cycle.
Call the next middleware function in the stack.

### What is the req object?

The req object represents the HTTP request that was received by the Express app

### What is the res object?

The res object represents the HTTP response that the Express app sends when it gets an HTTP request

### Why is next important?

The next middleware function is important as it tells express to move to the next middleware in the stack, forgetting to call next when your middleware function does not send a response back to the client then your app will pause. 

### What does app.use do?

App.use loads your middleware function