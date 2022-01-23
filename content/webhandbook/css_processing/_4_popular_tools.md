---
title: 4 Popular Tools
---

There are four very popular CSS processing tools. They all support some of the features mentioned above, but none of them support them all. Further, some of them can be used together, but again not all.

### Sass

Sass[10] is the oldest of the four presented tools, with the initial release in 2006. It has a large set of features that extend the CSS syntax, like nesting, functions or variables, and supports two syntaxes. The original syntax (syntactically awesome style sheets, `.sass`), uses indention and line breaks instead of curly braces and semicolons. Later another syntax was added that is similar to CSS block formatting (Sassy CSS, `.scss`).

### Less

The Less[11] processor was created after Sass, and as such, they have near feature-parity. The language was designed to be very close to CSS and, CSS block formatting syntax. Even though Less can be precompiled to CSS as the other tools, it is also possible to ship and run the compiler in the browser.

While Sass uses `$` to denote variables, Less employs `@`-symbols, which has the drawback that some parts of the modern CSS spec, such as media queries or animations, also use it for other purposes, which can be confusing.

### Stylus

The third stylesheet processor that appeared in 2010 and is influenced by Sass and Less is Stylus[12], hence the set of features is very similar. The big differentiator of Stylus is its minimalist syntax, which makes line-breaks, and semicolons optional, comparable to Sass, and even go a step further and makes colons optional as well.

Stylus adoption is relatively low in comparison to Sass and Less[13]. Especially built-in support in IDEs, Editors and bundlers is lower. But most popular development tools have extensions available.

### PostCSS

PostCSS[14] is different from the previous tools in so far that it is less a CSS processor in of itself, and instead a framework with which plugins can modify CSS. First, the input CSS is parsed into a syntax tree on which plugins can perform modifications, once they are done PostCSS transforms the modified tree back into CSS.

The default parser for PostCSS can only parse CSS; foreign syntax, as it is introduced by Less, Sass or Styles first needs to be compiled down to CSS. Therefore, it is not uncommon that PostCSS is used in conjunction with one of these languages. Also, due to the available range of plugins PostCSS can not only be used for minification and auto prefixing, but also as a linter or formatter.
