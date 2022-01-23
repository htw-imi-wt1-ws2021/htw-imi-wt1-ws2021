---
title: 5 Integration and Considerations
---

### Integration

The presented processing tools all come with command-line interfaces, which take multiple input files and usually a config to generate or transform CSS.

Usually, these transformations are done in a more complex build pipeline for the entire project, using a bundler or task-runner. Especially Sass and Less have multiple implementations in different languages. Which one is most suitable often depends on the bundler or task-runner that is being used.

### Considerations

CSS processors are optional tools that offer a wide array of capabilities for different parts of a web project. Because many modern web projects use a bundler or task-runner already, including these tools is mostly trivial.

Optimizations such as minification are easy to integrate and can instantly improve a web page's performance. They don't require the adaption of a different language or different patterns.

On the other hand, Authoring features are only as good as how they are used. If a project can benefit from these features has to be assessed the same way other programming patterns and frameworks are.
