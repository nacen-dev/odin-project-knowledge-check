# ES6 Modules

## Knowledge Check

### Explain what npm is and where it was commonly used before being adopted on the frontend.

NPM is a package manager used to help automate downloading, and upgrading of libraries from a repository. It was built specifically for node.js, a JavaScript Runtime Environment designed to run on a server.

### Describe what npm init does and what package.json is.

NPM init is a command to initialize a package.json file it will ask you certain question so it can fill the required values in package.json

A package json file

- lists the packages your project depends on
- specifies versions of a package that your project can use using semantic versioning rules
- makes your build reproducible, and therefore easier to share with other developers

### Know how to install packages using npm.

Using the `npm install` command

### Describe what a JavaScript module bundler like webpack is.

A JavaScript module bundler is a tool solves the problem where the browser do not have access to the file system in and since the browser do not have access to the file system loading modules becomes tricky, the module bundler solves that by taking the javascript file and their dependencies the `modules` and bundle them into a single file.

### Explain what the concepts “entry” and “output” mean as relates to webpack.

Entry is where webpack will start bundling the file and output is where it will produce an output of the bundled file

### Briefly explain what a development dependency is.

A development dependency is a dependency that the project requires during the development phase these packages are necessary in development but not in production build, some example would be plugins, presets, test runners, linter and etc.

### Explain what “transpiling code” means and how it relates to frontend development.

Transpiling code is converting the code in one language to code in another similar language. It relates to frontend development as browsers are slow to add new features by transpiling the code we can use new features that eventually gets translated to code that is browser-compatible.

### Briefly describe what a task runner is and how it’s used in frontend development.

A task runner is a tool to automate different parts of the build process like minifying code, optimizing images, running test, and etc.

### Describe how to write an npm automation script.

Going to the package.json file you will see a script object and inside you can enter the script name to call and what it should do when it gets called for example

```
"scripts": {      
  "test": "echo \"Error: no test specified\" && exit 1",      
  "build": "webpack --progress -p",      
  "watch": "webpack --progress --watch",
  "serve": "webpack-dev-server --open"
  },
```

when we run npm run build it is equivalent to running webpack --progress -p in the command line.

### Explain one of the main benefits of writing code in modules.

One of the main benefits of writing code in modules is `code reuse`.

### Explain “named exports” and “default exports”.

named exports are exported function, variable that are named and must be imported using that name, a default export is an export that is automatically imported even if you do not specify its name.
