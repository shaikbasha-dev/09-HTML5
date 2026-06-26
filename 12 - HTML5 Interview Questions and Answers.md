# Top 100 HTML5 Interview Questions & Answers

This document compiles 100 essential HTML5 interview questions and detailed answers, categorized logically from foundational structure up to advanced APIs and browser optimization practices. Perfect for revision, interviewing, or technical onboarding.

---

## Table of Contents
1. [Core Structure & Semantic Elements (1-10)](#1-core-structure--semantic-elements)
2. [Multimedia & Streaming Elements (11-20)](#2-multimedia--streaming-elements)
3. [Graphics, Canvas & SVG (21-30)](#3-graphics-canvas--svg)
4. [Form Enhancements & Input Controls (31-50)](#4-form-enhancements--input-controls)
5. [Client-Side Web Storage & Workers (51-70)](#5-client-side-web-storage--workers)
6. [Advanced Browser APIs & Interactive Layouts (71-85)](#6-advanced-browser-apis--interactive-layouts)
7. [Script Optimization, Best Practices & Validation (86-100)](#7-script-optimization-best-practices--validation)

---

## 1. Core Structure & Semantic Elements

### Q1: What is HTML5 and how does it differ from HTML4?
**Answer:**
HTML5 is the latest major revision of the Hypertext Markup Language. Key differences include native support for audio/video (`<audio>`, `<video>`), new semantic elements (`<header>`, `<footer>`, `<article>`), drawing capabilities via `<canvas>`, localized storage (`localStorage`/`sessionStorage`), and the removal of deprecated elements like `<font>`, `<center>`, and `<strike>`.

### Q2: What are semantic elements in HTML5?
**Answer:**
Semantic elements clearly describe their meaning to both the browser and the developer. Examples include `<article>`, `<aside>`, `<details>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<section>`, and `<summary>`.

### Q3: Why should we use semantic tags instead of generic <div> tags?
**Answer:**
Semantic tags improve Accessibility (SEO engines and screen readers understand structure better), enhance Maintainability (code is easier to read and structure), and follow modern web standards without relying on arbitrary class names like 'header' or 'footer'.

### Q4: What is the purpose of the <!DOCTYPE html> declaration in HTML5?
**Answer:**
It is a required instruction to the web browser about what version of HTML the page is written in. In HTML5, it is intentionally short and simple, forcing the browser to render the page in standard compliance mode instead of quirks mode.

### Q5: What is the purpose of the <main> tag?
**Answer:**
The `<main>` tag specifies the dominant content of the `<body>` of a document. The content inside `<main>` should be unique to the document and should not contain content that is repeated across pages, such as sidebars, navigation links, or copyright information. A document must not include more than one `<main>` element.

### Q6: Explain the difference between <section> and <article>.
**Answer:**
`<article>` represents a self-contained, independent piece of content that could be reused or distributed independently (e.g., a blog post, news article, forum post). `<section>` represents a thematic grouping of content, typically with a heading, used to break up a larger page into logical parts.

### Q7: What is the purpose of the <aside> tag?
**Answer:**
The `<aside>` element defines content that is tangentially related to the content around it, like sidebars, callout boxes, advertising blocks, or related links.

### Q8: What does the <figure> and <figcaption> tag do?
**Answer:**
The `<figure>` tag specifies self-contained content, like illustrations, diagrams, photos, or code listings. The `<figcaption>` tag defines a caption or explanation for that element and is placed as the first or last child of the `<figure>` component.

### Q9: What is the purpose of the <header> and <footer> tags?
**Answer:**
`<header>` represents a container for introductory content or a set of navigational links (often containing an `<h1>`-`<h6>`, logo, or search form). `<footer>` represents a footer for its nearest sectioning content, typically containing authorship information, copyright data, links to privacy policies, etc.

### Q10: What is the <nav> element used for?
**Answer:**
The `<nav>` element defines a block of navigation links designed specifically for major navigation blocks on a website, allowing screen readers to skip or target navigation easily.

## 2. Multimedia & Streaming Elements

### Q11: What are the new media elements introduced in HTML5?
**Answer:**
HTML5 introduced native multimedia elements: `<video>` for video playback, `<audio>` for audio streams, and `<embed>` / `<source>` to act as containers for external resources or multiple media formats.

### Q12: How do you provide alternative media streams for browsers that don't support a specific format?
**Answer:**
By nesting multiple `<source>` elements inside a `<video>` or `<audio>` element. The browser will use the first recognized format. For example:
```html
<video controls>
  <source src='movie.mp4' type='video/mp4'>
  <source src='movie.ogg' type='video/ogg'>
  Your browser does not support the video tag.
</video>
