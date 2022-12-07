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
  - [HTML5 Latest Tag](#html5-latest-tag)
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
- [Web Accessibilities](#web-accessibilities)
- [W3C Validation](#w3c-validation)
- [JavaScript](#javaccript)
  - [How JavaScript Work](#how-javascript-work)
  - [Context API](#context-api)
  - [Event Loop](#event-loop)
  - [DOM Manipulation](#dom-manipulation)
  - [Asynchronous JavaScript](#asynchronous-javascript)
    - [Callback](#callback)
    - [Promese](#promese)
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
  - [What is ReactJS Fibar](#what-is-reactjsfibar)
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

    HTML sanitization generally refers to removing potentially malicious JavaScript content from raw HTML strings

    **[⬆ Back to Top](#advanced-front-end-preparation-guide)**
