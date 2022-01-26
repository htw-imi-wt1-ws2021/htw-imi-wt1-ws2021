---
title: 2 Types of Render Modes and their Advantages and Disadvantages
description : "Types of Render Modes and their Advantages and Disadvantages"
tags: ["render modes", "advantages", "disadvantages", "rendering"]
---

### Rendering Modes


* [Traditional SSR (Server Side Rendering)](#traditional-ssr-server-side-rendering)
* [Traditional SPA (Single Page Application) using CSR (Client Side Rendering)](#traditional-spa-single-page-application-using-csr-client-side-rendering)
* [Universal / Rehydration SSR](#universal--rehydration-ssr)
* [Static SSR](#static-ssr)
* [CSR with Pre-Rendering](#csr-with-pre-rendering)



## **TRADITIONAL SSR** (SERVER SIDE RENDERING)

Server Side Rendering was the only way to do things when the web just started. The server generates all HTML files and sends it to the browser – so the browser gets a fully formed HTML web page with the HTML components already created. The browser now only has to parse the HTML to generate the DOM and display the website. With every request from the browser, all the scripts, styles and templates have to be sent from the server to the client (the browser) again.
Server Side Rendering can be done at build time, which pre-generates the HTML, or at request time for each incoming request from the browser, also known as Dynamic SSR.

__Examples__

Websites using PHP, ASP.NET, Java or Ruby are normally built using traditional SSR.

__Advantages__

* __Better SEO performance:__ The client receives the finished page with all the data and HTML tags, especially the meta tags that belong to the page, so search engines can crawl the page and index it.
* __Faster initial load time:__ The client only has to parse the content, which is faster than having to render it.
* __Also visible when JS is disabled:__ Since all the HTML is generated on the server-side, the website will be displayed correctly even if JS is disabled.

__Disadvantages__

* __Poor responsiveness and user experience with bad internet connectivity:__ Re-
rendering takes time and the user has to wait for each request to complete – when there is bad internet connection, it might take a while to see new content.


## **TRADITIONAL SPA** (SINGLE PAGE APPLICATION) USING CSR (CLIENT SIDE RENDERING)

The complete opposite to Traditional SSR is a Single Page Application that is client-side rendered. In CSR, the HTML components are generated on the client-side by executing JavaScript in the browser. On initial request, the server only returns a minimal HTML page (therefore the name _Single Page Application_) that serves as the application container. The browser must then fully download the JS bundle linked in the HTML and run the JS in the browser, which in turn creates the HTML DOM on the client-side. Further interactions only happen on the client-side and no request is sent to the server.

__Examples__

Traditional React or Vue Applications are fully CSR.

__Advantages__

* __Super fast and responsive after initial load:__ There are no round trips to the server which fastens up loading times significantly.
* __Easier development and deployment:__ No server is needed and the HTML, JS and CSS can just be dropped to a remote server and go live right away.

__Disadvantages__

* __Not SEO friendly:__ The SPA content is loaded via JS that the crawlers mostly cannot execute, and therefore they only see the bare single HTML pages with almost no content.
* __Slow initial load time:__ Most resources like the CSS, JS and HTML templates are loaded once at the initial load of the app, so it’s rather slow when first being opened.
* __JS has to be enabled:__ You will see a blank page if JS is disabled because the JS bundle will never run on the client and so the HMTL will not get generated, therefore the webpage will not be rendered.


## **UNIVERSAL / REHYDRATION SSR**

Universal SSR tries to combine the advantages of Traditional SSR and Traditional CSR. This becomes possible through the fact that JS has become an isomorphic language since the release of Node.js in 2009, which means that the code can run on the client and the server side. In Universal SSR, the app will pre-load on the server, pre-render the pages and react to navigation requests like full page loads and reloads and send the rendered HTML to the browser. The client then takes control and Rehydration (also called „Hydration“) happens: the JS bundle gets downloaded in the background and event handlers get attached to the pre-rendered static HTML. So from now on the application acts like a SPA.

__Examples__

Nuxt SSR (Vue), Next SSR (React), Gatsby SSR (React)

__Advantages__

* __Faster initial load time:__ As pages are pre-rendered, the initial load time is higher as with traditional CSR
* __Better SEO results:__ Again, because of the pre-rendering, search engine crawlers can scan the content of the page
* __Better user experience:__ Faster initial reaction and seamless transitions between pages: the user experience profits from the combination of SSR and CSR

__Disadvantages__

* __Server required:__ A Node.js server is required to run JS on the server
* __Complex development:__ Combining server and client JS can be confusing because some plugins and libraries are only meant to run on the client side and you have to be careful what you can use.


## **STATIC SSR**

Apps that are static-generated are pre-generated with the help of a Static Site Generator (SSG). All pages are pre-rendered at build time to static HTML files that will be stored on a static hosting server. No JS is executed on the browser anymore because this is already done on the server, the website is completely static on the client, but it still acts like a SPA.

__Examples__

Next Static HTML Export (React), Hugo, Gatsby SSG (React), Jekyll, Metalsmith

__Advantages__

* __Faster initial load time:__ As pages are pre-generated as static HTML, the initial load time is very fast
* __SEO friendly:__ All JS can be crawled by search engines, like in traditional SSR apps
* __Easy and fast deployment:__ Numerous static hosting servers are available for fast deploys
* __Works with JS disabled:__ As no JS is executed on the browser, the website still looks and behaves the same if JS is disabled

__Disadvantages__

* __HTML files must be generated for every possible URL:__ this can be challenging if you can’t predict what those URLs will be or for sites with a large number of unique pages
* __No real-time rendering:__ Static generated sites can only display content that was pre- rendered during build time. If real-time rendering is required, universal SSR should be used.


## **CSR WITH PRE-RENDERING**

It’s easy to confuse Static SSR with Pre-Rendering: in both cases, HTML files are statically generated during build time. With Pre-Rendering the difference is that only partials of the HTML, the initial skeleton, is pre-rendered. Once the files are sent to the browser, hydration takes over again and then the application acts like a full SPA. How’s
this different to Universal SSR then? The difference is that it doesn’t need a server for further requests, everything happens on the client like in a Traditional CSR. Only the initial load time is enhanced for better user experience.

__Examples__

Nuxt Static Site Generator (Vue), Gatsby, Vuepress

__Advantages__

* __Fast Initial Load Time:__ Pages are partially pre-generated so the initial load time decreases.
* __Better SEO:__ As pages are pre-rendered, the initial state and content can be captured by search engine crawlers

__Disadvantages__

* __Does not work if JS is disabled:__ some basic functionality may still exist, but most of the page will be useless