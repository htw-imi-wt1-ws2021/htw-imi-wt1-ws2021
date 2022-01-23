---
title: 1 History and Terminology
---

### History

CSS processors have existed for quite a while. The first release of the popular Sass processor was in 2006! CSS is a powerful and versatile language to describe the appearance of web pages but lacks features from other programming languages to increase productivity and reduce redundancies. However, some shortcomings of the language have been addressed in recent years, and features that once could only be achieved through CSS processors are now available in the language itself.

For instance, when Sass was first released, there was no concept of variables in CSS, and values such as colors had to be hardcoded everywhere. So when large web projects wanted to change a specific color (e.g., the brand color), they had to go through all their stylesheets and replace the old values with the new ones.

Modern CSS has native support for variables and many other features that once were only available through CSS processors. But not everything CSS processors have to offer exists in CSS today, and some will never be able to.

### Terminology

When talking about CSS processing, typically, there is a separation between pre-processing and post-processing. The former describes transforming something that is not CSS into spec-compliant CSS, and the latter takes already valid CSS and optimizes it in some fashion. However, the most popular tools that perform these transformations can not be distinctly classified as falling clearly into one of these two categories anymore since they support functions that fall both into pre- and post-processing.

In his article 'Deconfusing Pre- and Post-processing' [1], Stefan Baumgartner defines a different terminology, authoring and optimization, instead of pre-and post-processing to classify the various features of CSS processing tools. This new categorization still doesn't allow us to neatly assign any feature to precisely one of the two categories. Still, it generally makes it easier to discuss whether something helps developers write nicer code or is done to optimize for size or greater support.
