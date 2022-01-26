---
title: 1 Fundamentals of Website Rendering
description : "Fundamentals of Website Rendering"
tags: ["fundamentals", "rendering"]
---

To display the contents of a website, a browser will typically request HTML, CSS, JavaScript and image content from a server and interpret it based on web standards and specifications. While doing so it uses multiple engines, each with different tasks that it has to complete. For example there is the Layout Engine that reacts to user input e.g. in the URL bar, or there is the Network Layer that handles network functions and all kinds of network requests.

The **Rendering Engine** is responsible for displaying the contents on our screen. It has to communicate with the network layer to get the HTML code and other things passed from a remote server. 
Then it follows several steps:

1. It parses the HTML to construct the **DOM** (Document Object Model, which represents the website in a tree structure, where every node is an object corresponding to a part of that website).
2. The styles are loaded and parsed into the **CSSOM** (CSS Object Model, contains all the selectors and selector properties needed to correctly render the page).
3. The **render tree** is created using the DOM and CSSOM.
4. The **layout process** takes place, where the engine scans which object should be
placed where.
5. Lastly, the information is **painted** and appears on our screen in the browser.
Traditionally, JavaScript only gets executed after the web page has been rendered and painted to the screen and triggers a re-render if changes happen. Web crawlers that scan your website therefore often struggle with content that loads dynamically. But because SEO and the visibility of a website is oftentimes very important, new solutions moving away from the traditional way of website rendering have evolved. They will be explained now.