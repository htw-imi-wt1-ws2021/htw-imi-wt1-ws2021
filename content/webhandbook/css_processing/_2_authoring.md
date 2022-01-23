---
title: 2 Authoring
---

As mentioned in the previous chapter, the CSS specification has significantly caught up with the feature set that processing tools provide today. Features such as variables, color mixing, importing, or mathematical operations can all be used directly in the browser with the added benefit of being dynamically changeable.[2]

Still, there are CSS processor features that can immensely help with writing nice code and that have not made it in the CSS spec. In addition, many larger web applications use processing tools to optimize their CSS for production — more on that later — so adding additional tools that aid with the authoring of stylesheets is relatively easy. Another reason to use the authoring features provided by these tools may be to target older browsers that lack support for these features.

It is crucial to remember that CSS processors can only perform operations on the static stylesheet before they are sent to and evaluated by the browser. This "static compilation" can be helpful, as it allows for complicated syntax extensions that simply compile to regular CSS. The downside is, because this compilation happens before the stylesheet is evaluated it also means that there is no context for the state of the environment. For instance, modern CSS's math capabilities allow adding absolute units to relative ones, so `height: calc(100% + 32x)` is perfectly valid. The same does not work with CSS processors, even though they also have math operations, since the calculation has to resolve at compile-time, and the width of 100% is unknown.[3]

### Nesting

One widely used feature that has not made it into the CSS specification is nesting. Nesting allows developers to write one style rule within another. For instance, instead of having to write:

```css
ul {
    margin: 0;
}
ul li {
    display: inline-block;
}
ul a {
    text-decoration: none;
}
```

Developers can write the following to increase legibility and avoid unnecessary repetition:

```scss
ul {
    margin: 0;
    li {
        display: inline-block;
    }
    a {
        text-decoration: none;
    }
}
```

### Parent Selector

One handy feature that comes with nesting, which can improve legibility, is the parent selector, with which the outside selector can get referenced and extended. An ampersand denotes this parent selector. So, for example, instead of writing:

```scss
button {
    background: lightgrey;
}
button:hover {
    background: gray;
}
```

Developers can write:

```scss
button {
    background: lightgray;
    &:hover {
        background: gray;
    }
}
```

Nesting can reduce code repetition and visual clutter, but the generated CSS quickly increases. While nesting looks nicer to the developer, the CSS processor has to unnest the code again during compilation for it to become valid CSS again. To prevent unnecessarily specific and therefore large CSS selector rules, keeping the nesting depth as shallow as possible is recommended.[4]

### Mixins

CSS Processors also bring simple control flow statements and functions to stylesheets, common in other programming languages. This functionality allows writing reusable code patterns. For instance, instead of writing the following statement again and again:

```scss
.background {
    top: 0px;
    left: 0px;
    bottom: 0px;
    right: 0px;
}
```

With what is called mixins in SASS, but is also available with other CSS processors, this statement can be made into a reusable function and then applied where necessary:

```scss
@mixin position($p) {
    top: $p;
    left: $p;
    bottom: $p;
    right: $p;
}
.background {
    @include position(0px)
}
```

### Different Syntax

CSS Processors can extend the existing CSS syntax and change it completely. Most notably, the Stylus language makes curly braces, semicolons, and colons optional in a stylesheet and hierarchy inferred by indentation, similar to python. This means instead of writing:

```scss
button {
    background: lightgray;
    &.primary {
        background: lightblue;
    }
}
```

the same rule in Stylus can get described like this:

```stylus
button
    background lightgray
    &.primary
        background lightblue 
```

### Modules

Nesting can be a great way to limit the scope of specific CSS rules, as in general, everything on a page shares the same scope. Another option to limit CSS rules to certain components using CSS processors is to use css-modules[5]. The idea is that CSS selectors can stay simple, shallow and concise, and then get automatically renamed to be unique to a module. For instance, a CSS class written as `.name` might be renamed in the final output to `.name_SVK0go`. Since this CSS processing feature changes the class names, integration with the HTML code is necessary, which adds considerably more complexity to the build pipeline than just converting the stylesheets.
