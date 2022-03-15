# Frameworks and Preprocessors

## Knowledge Check

### What are some advantages of using a CSS framework?

- Well made documentation

- Online Communities to help you

- The grid system

- Speed of project delivery

### What are some disadvantages of using a CSS framework?

- Difficulty of overriding the framework's code

- Website tends to look the same

- Performance Issues

- Technical Debt


### What are some advantages of using a CSS preprocessor?

- It makes your code adhere to the DRY principle (Do not repeat yourself)

- Makes code easier to maintain

- Makes code more organized

### What are some disadvantages of using a CSS preprocessor?

1. Debugging is harder

Preprocessors have a compilation step, meaning that CSS line numbers are irrelevant when trying to debug our code. But debugging is twice as hard as programming, so this alone is a huge drawback.

Source maps provide a solution, but they need to be setup and they don’t work in all browsers, particularly those where bugs often come up.

Without source maps, we’re left to search for rules in the hope that we find what we’re looking for.

2. Compilation slows down development

Compilation times can be really slow, even when using the best tools on the fastest computer. You know that feeling you get when you refresh and don’t see any changes—that.

3. They can produce very large CSS files

Source files may be small, but the generated CSS could be huge which is what counts.

We need to be aware that in using a CSS preprocessor, we’re losing some control.

4. Maintenance and over-engineering

It’s common to see coder authors using a red variable, for example. But this is of little value in terms of maintainability.

If the colour changes, then we need to update the name and the value, making the abstraction pointless.

Not only are there alternatives to variables and mixins, which I’ll cover later, but a search and replace maybe all we need.

5. Tooling and developer convenience

CSS preprocessors require extra tooling. Code authors shouldn’t be forced to use a particular editor just to be able to use the tool. That’s the tail wagging the dog.

Also, extra stuff adds complexity. This needs to be understood, upgraded and maintained—all of which increases cost and a higher risk of problems.

6. Saving generated files (or not)

Whether we should save the generated CSS or not is something we don’t agree on as a community. In which case, it’s time for some Concensus Driven Development.

7. Capability and understanding

Whilst CSS preprocessors and the workflows around them have become widespread, there is still a knowledge gap. Particularly, when it comes to understanding the trade-offs.

There’s a big difference between understanding a tool, and using it effectively without introducing other problems.