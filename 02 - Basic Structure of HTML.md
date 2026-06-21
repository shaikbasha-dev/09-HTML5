# 02 - Basic Structure of HTML

Every HTML document follows a standard structure. This structure helps browsers understand and render the web page correctly.

## Basic HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    <p>Welcome To HTML</p>
</body>
</html>
```

---

## Tags Used in Basic HTML Structure

The above HTML document contains the following tags:

1. `<!DOCTYPE html>`
2. `<html></html>`
3. `<head></head>`
4. `<title></title>`
5. `<body></body>`
6. `<p></p>`

---

## 1. <!DOCTYPE html>

### Definition

`<!DOCTYPE html>` is called the **Document Type Declaration**.

It tells the browser that the document is written in HTML5.

### Purpose

* Informs the browser to use HTML5 standards.
* Ensures the browser renders the page correctly.
* Must always be the first line of an HTML document.

### Syntax

```html
<!DOCTYPE html>
```

### Example

```html
<!DOCTYPE html>
```

---

## 2. `<html lang="en"></html>`

### Definition

The `<html>` tag is called the **Root Element** of an HTML document.

It contains all other HTML elements.

### lang Attribute

```html
lang="en"
```

The `lang` attribute specifies the language of the web page.

Here:

* `en` means English.

### Purpose

* Acts as the root container of the document.
* Helps search engines understand page language.
* Improves accessibility.

### Syntax

```html
<html lang="en">

</html>
```

### Example

```html
<html lang="en">

</html>
```

---

## 3. `<head></head>`

### Definition

The `<head>` tag contains metadata about the HTML document.

Metadata means information about the webpage that is not displayed directly on the browser page.

### Purpose

The `<head>` section contains:

* Title of the page
* Meta tags
* CSS links
* JavaScript links
* Icons (Favicons)

### Syntax

```html
<head>

</head>
```

### Example

```html
<head>
    <title>My Website</title>
</head>
```

---

## 4. `<title></title>`

### Definition

The `<title>` tag specifies the title of the webpage.

The title is displayed:

* On the browser tab.
* In search engine results.
* In bookmarks.

### Syntax

```html
<title>

</title>
```

### Example

```html
<title>HTML Basics</title>
```

Output:

Browser Tab:

```text
HTML Basics
```

---

## 5. `<body></body>`

### Definition

The `<body>` tag contains all the visible content displayed on the browser.

Everything visible to the user is written inside the `<body>` tag.

### Examples of Content

* Headings
* Paragraphs
* Images
* Tables
* Forms
* Videos
* Links

### Syntax

```html
<body>

</body>
```

### Example

```html
<body>

<h1>Welcome</h1>

<p>This is HTML.</p>

</body>
```

---

## 6. `<p></p>`

### Definition

The `<p>` tag is called the **Paragraph Tag**.

It is used to display paragraphs of text on a webpage.

### Purpose

* Displays text in paragraph format.
* Automatically adds spacing before and after the paragraph.

### Syntax

```html
<p>

</p>
```

### Example

```html
<p>Welcome To HTML</p>
```

Output:

```text
Welcome To HTML
```

---

## Complete Explanation of the Program

```html
<!DOCTYPE html>
```

Declares the document as an HTML5 document.

---

```html
<html lang="en">
```

Starts the HTML document and specifies English as the language.

---

```html
<head>
```

Starts the metadata section.

---

```html
<title>Document</title>
```

Sets the browser tab title as "Document".

---

```html
</head>
```

Ends the metadata section.

---

```html
<body>
```

Starts the visible content section.

---

```html
<p>Welcome To HTML</p>
```

Displays a paragraph on the webpage.

---

```html
</body>
```

Ends the body section.

---

```html
</html>
```

Ends the HTML document.

---

## Important Points

* `<!DOCTYPE html>` should always be the first line.
* `<html>` is the root element.
* `<head>` contains metadata.
* `<title>` defines the browser tab title.
* `<body>` contains visible content.
* `<p>` is used to display paragraphs.

---

## Summary

The basic structure of HTML is the foundation of every webpage. Every HTML document starts with `<!DOCTYPE html>` followed by the `<html>`, `<head>`, and `<body>` tags. Understanding this structure is essential before learning advanced HTML elements and web development concepts.
