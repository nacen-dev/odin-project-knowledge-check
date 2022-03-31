# Working with API's

### What is an API?

An API is a server that serves data for external use(websites or apps), it stands for `Application Programming Interface`

### How is access to an API restricted?

An API is restricted by using an API Key, the API can track how many request you use in your application so they can track abuse of their systems and data.

### How do you fetch and extract data from an API?

There are multiple ways to fetch and extract data from an API, but my answer would be using the native fetch API which provides a simple way to fetch and extract data.

### Why might your API request be blocked by the browser, and how might you fix this?

Because of security reasons the browser by default restricts HTTP requests to outside sources, for now what I learned to bypass this is to supply another argument to the fetch function by adding an object that has a method property which has a value of 'cors

```
fetch('url.url.com/api', {
  mode: 'cors'
});
```