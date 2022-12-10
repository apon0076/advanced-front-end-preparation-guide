# Advanced Front End Preparation Guide

    Table of Content

- [HTML](#html)
  - [Semantic HTML](#semantic-html)  
     Q1. [What are Semantic Elements?](#what-are-semantic-elements)  
     Q2. [Examples of Some Semantic Elements.](#examples-of-some-semantic-elements)  
     Q3. [Why Should We Use Semantic Tags Instead of Generic Tags?](#why-should-we-use-semantic-tags-instead-of-generic-tags)  
     Q4. [How Semantic HTML Helps in SEO?](#how-semantic-html-helps-in-seo)  
     Q5. [How Semantic HTML Helps in Accessibility?](#how-semantic-html-helps-in-accessibility)
  - [HTML Sanitization](#html-sanitization)  
     Q6. [What is HTML Sanitization?](#what-is-html-sanitization)  
     Q7. [Types of HTML Sanitization](#types-of-html-sanitization)  
     Q8. [Name Some Libraries for Clients Side Sanitization](#name-some-libraries-for-clients-side-sanitization)
  - [HTML5 Latest Tag](#html5-latest-tag)  
     Q9. [What is HTML5?](#what-is-html5)  
     Q10. [New Features of HTML5?](#new-features-of-html5)  
     Q11. [Latest Tags of HTML5?](#latest-tags-of-html5)
- [CSS](#css)
  - [Flexbox](#flexbox)
  - [Grid](#grid)
  - [SCSS](#scss)
  - [Naming Convention](#naming-convention)
    - [BEM](#bem)
    - [ABEM](#abem)
  - [Folder Structure](#folder-structure)
    - [ITCSS](#itcss)
  - [Modular CSS](#modular-css)
  - [Object Oriented CSS](#object-oriented-css)
- [Web Accessibility](#web-accessibility)
- [W3C Validation](#w3c-validation)
- [JavaScript](#javaccript)
  - [How JavaScript Work](#how-javascript-work)
  - [Context API](#context-api)
  - [Event Loop](#event-loop)
  - [DOM Manipulation](#dom-manipulation)
  - [Asynchronous JavaScript](#asynchronous-javascript)
    - [Callback](#callback)
    - [Promise](#promise)
    - [Async and Await](#async-and-await)
  - [Webpack](#webpack)
- [Testing](#testing)
  - [Unit Testing](#unit-testing)
    - [JEST](#jest)
    - [React Testing Library](#react-testing-library)
  - [Integration Testing](#integration-testing)
    - [JEST](#jest)
    - [React Testing Library](#react-testing-library)
  - [E2E Testing](#e2e-testing)
    - [Puppeteer JS](#puppeteer-js)
    - [Playwright](#playwright)
- [ReactJS](#reactjs)
  - [How React JS Work](#how-react-js-work)
  - [How Virtual DOM Actually Work](#how-virtual-dom-actually-work)
  - [What is ReactJS Fiber](#what-is-reactjs-fiber)
- [ReactJS Packages](#reactjs-packages)
  - [State Management](#state-management)
  - [Story Book](#story-book)
  - [React Query](#react-query)
  - [MaterialUI](#materialui)
- [TypeScript](#typeScript)
- [Data Structure and Algorithm](#data-structure-and-algorithm)
  - [Complexity Analysis](#complexity-analysis)
    - [Time Complexity](#time-complexity)
    - [Space Complexity](#space-complexity)
  - [Data Structure](#data-structure)
    - [Linear Data Structure](#linear-data-structure)
    - [Non-Linear Data Structure](#non-linear-data-structure)
  - [Algorithm](#algorithm)
    - [Searching](#searching)
    - [Sorting](#sorting)
    - [Tree](#tree)
    - [Graph](#graph)
    - [Dynamic Programming](#dynamic-programming)

## HTML

- ### Semantic HTML

1.  ### What are Semantic Elements?

    A semantic element clearly describes its meaning to both the browser and the developer.  
    Examples of non-semantic elements: `<div> and <span>` - Tells nothing about its content.  
    Examples of semantic elements: `<form>, <table>, and <article>` - Clearly defines its content.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

2.  ### Examples of Some Semantic Elements.
    ```
    <article>
    <aside>
    <details>
    <figcaption>
    <figure>
    <footer>
    <header>
    <main>
    <mark>
    <nav>
    <section>
    <summary>
    <time>
    ```
    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**
3.  ### Why Should We Use Semantic Tags Instead of Generic Tags?

    Semantic tags provide meaning to the content they contain, whereas generic tags do not. This meaning can be interpreted by both humans and machines, which can be helpful in a number of ways. For example, screen readers can use the semantic information in a document to provide a more meaningful experience for blind or visually impaired users. Search engines can also use semantic information to provide more relevant results for users. In general, using semantic tags makes your HTML code more understandable and easier to work with.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

4.  ### How Semantic HTML Helps in SEO?

    Semantic HTML refers to syntax that makes the HTML more comprehensible by better defining the different sections and layout of web pages. It makes web pages more informative and adaptable, allowing browsers and search engines to better interpret content

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

5.  ### How Semantic HTML Helps in Accessibility?

    Semantic HTML gives context to screen readers, which read the contents of a page out loud. With the button example in mind: buttons have more suitable styling by default. a screen reader identifies it as a button.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

- ### HTML Sanitization

6.  ### What is HTML Sanitization?

    HTML sanitization generally refers to removing potentially malicious JavaScript content from raw HTML strings.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

7.  ### Types of HTML Sanitization

    There are two different HTML sanitization implementations:

    i) Client-side sanitization: prevents unsafe content from the DOM level  
    ii) Server-side sanitization: prevents the storage of malicious HTML content in databases

    We indeed need to use both sanitization layers to prevent XSS vulnerabilities. If your database is affected by malicious XSS payloads, the client-side sanitization layer will protect all application users, but if an attacker sends malicious HTML directly from the RESTful API, server-side sanitization will protect the system.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

8.  ### Name Some Libraries for Clients Side Sanitization

    Web developers tend to use the following libraries for client-side/DOM-level sanitization:

    i) `DOMPurity`: HTML sanitizer library for JavaScript, that also works on server-side Node.js via the `jsdom` package

    ii) `js-xss`: An HTML sanitizer library that works on browser, server-side `Node.js`, and as a command-line tool

    iii) `sanitize-html`: An htmlparser2-based sanitizer library for `Node.js` and browser that’s very popular among React developers because there is a wrapper library especially for React

    These libraries typically parse unsafe HTML using either the browser’s inbuilt DOM iterator, or a custom HTML parser that excludes unsafe HTML content before using `innerHTML`.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

9.  ### What is HTML5?

    HTML5 is a markup language used for structuring and presenting content on the World Wide Web. It is the fifth and final major HTML version that is a World Wide Web Consortium (W3C) recommendation. The current specification is known as the HTML Living Standard.

    It is maintained by the Web Hypertext Application Technology Working Group (WHATWG), a consortium of the major browser vendors (Apple, Google, Mozilla, and Microsoft). It was initially released on 22 January 2008.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

10. ### New Features of HTML5?

    HTML5 introduces a number of new elements and attributes that can help you in building modern websites. Here is a set of some of the most prominent features introduced in HTML5

    i) `New Semantic Elements` − These are like `<header>`, `<footer>`, and `<section>`.

    ii) `Forms 2.0` − Improvements to HTML web forms where new attributes have been introduced for `<input>` tag.

    iii) `Persistent Local Storage` − To achieve without resorting to third-party plugins.

    iv) `WebSocket` − A next-generation bidirectional communication technology for web applications.

    v) `Server-Sent Events` − HTML5 introduces events which flow from web server to the web browsers and they are called Server-Sent Events (SSE).

    vi) `Canvas` − This supports a two-dimensional drawing surface that you can program with JavaScript.

    vii) `Audio & Video` − You can embed audio or video on your webpages without resorting to third-party plugins.

    viii) `Geolocation` − Now visitors can choose to share their physical location with your web application.

    ix) `Microdata` − This lets you create your own vocabularies beyond HTML5 and extend your web pages with custom semantics.

    x) `Drag and drop` − Drag and drop the items from one location to another location on the same webpage.

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**

11. ### Latest Tags of HTML5?

    The following tags (elements) have been introduced in `HTML5` :

    <table>
    <tr>
    <th>
    ddd
    </th>
    </tr>
    </table>

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**
