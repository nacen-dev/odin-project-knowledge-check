# Authentication Basics

## Knowledge Check

### Which passportJS strategy did we use in this lesson?

Local strategy

### Why does passportJS create a cookie?

To make sure that the user is logged in and they stay logged in while moving through the app. passportJS will create a cookie to be stored in the browser.

### What does the bcrypt.compare() function do?

It compares the hashed password stored in the database with the plain text password that was sent by the client 

### Why should we include bcrypt when we begin a project?

It is a library that helps with hashing passwords including it at the beginning of the project is best since if you implement it later when there are already users in the database their password will no longer work since their password previously was stored in plain text.