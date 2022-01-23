---
title: 3 Optimisation
---

In addition to the features that support developers in designing stylesheets, there are also features of CSS processors that optimize existing CSS for speed and browser support.

### Minification

The probably most popular CSS processing feature is minification. Most programming languages include characters that are not strictly part of the syntax but increase legibility. This means whitespace characters primarily, and to a lesser extent, the variable names a developer has chosen. Most CSS minifiers strip away comments and whitespace characters, which can lead to a reduction in file size up to 50%. This does not necessarily correlate with a 50% speed improvement, especially since most web servers compress their responses anyway, but it makes a difference nonetheless. The fewer characters there are to read, the less there are to compress, decompress and finally parse by the browser.

A more complicated but not uncommon minification technique is also to minify class names. For example, a class called `.form-check-input` before minification might be reduced to very short identifiers, such as `.ab`. Similar to CSS modules, this method also requires integration with the HTML code in order to work.

### Polyfills

Besides file-size reduction, CSS optimization also includes modifications to improve compatibility among different browsers. For instance, one use case is to automatically make a website compatible with right-to-left languages instead of performing these optimizations manually. Another example might be that a developer wants to use the `#rrggbbaa` hex color notation that has been introduced in browsers recently, where the opacity can be included in the hex notation. If a developer wants to use this notation but also wants compatibility with an older browser that does not support this syntax, they can use CSS processors to replace them. In this specific example, the PostCSS Color Hex Alpha[6] plugin would do the following:

```css
body {
  background: #6ebd6ecc;
}
/* becomes */
body {
  background: rgb(110, 189, 110, 0.8);
}
```

### Vendor Prefixes

A subset of these compatibility features is the automatic addition of vendor prefixes. The idea behind prefixing certain CSS properties was to denote that their functionality was either experimental or not part of the standard, so they could be experimented with but would not be relied upon by web developers until they were properly standardized. Some of the most notable properties were `animation`, `transition`, `box-shadow` and even `border-radius` that were already implemented in most browsers, but only through these prefixes. This meant that to create a transition that works across all browsers did look like this:

```yaml
-webkit-transition: all 4s ease;
-moz-transition: all 4s ease;
-ms-transition: all 4s ease;
-o-transition: all 4s ease;
transition: all 4s ease;
```

Because some of these features were already almost universally available, web developers used them. Automatic prefixing became a popular CSS processing feature to reduce the labor of writing the same line up to five times, just with different prefixes. The most notable prefixing tool is autoprefixer[7], where developers can target the browser versions they intend to support and add necessary prefixes.

An analysis from Rob O'Leary in 2021 has revealed that the number of properties that require prefixes has steadily gone down in recent years[8], and nowadays, browser vendors put new features behind user-controlled flags instead[9]. Still, there are good reasons to use prefixing today, for instance, simply to make websites compatible with older browsers that require these prefixes. Additionally, there are CSS properties that have 99% browser support with prefixes and significantly less without[8], even if most or all of them might not be as relevant as the prefixed versions of `box-shadow` or `border-radius` once were.
