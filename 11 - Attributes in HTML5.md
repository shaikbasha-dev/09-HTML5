# 11 - Attributes in HTML5

## Introduction

Attributes provide additional information about HTML elements.

They define:

* Element behavior
* Element appearance
* Input validation
* External resource links
* Styling information
* Browser behavior

Attributes are always written inside the opening tag.

### Syntax

```html
<tagname attribute="value">
```

Example:

```html
<a href="https://www.google.com">Google</a>
```

Here:

* `href` is the attribute
* `https://www.google.com` is the value

---

# 1. Global Attributes

Global attributes can be used with almost every HTML element.

---

## id

### Definition

The `id` attribute defines a unique identifier for an element.

It is mainly used by:

* CSS
* JavaScript
* Labels
* DOM Manipulation

### Syntax

```html
<p id="intro"></p>
```

Example:

```html
<h1 id="heading1">Welcome To HTML5</h1>
```

---

## class

### Definition

The `class` attribute assigns one or more class names to an element.

It is used for:

* CSS Styling
* Grouping elements
* JavaScript selection

### Syntax

```html
<p class="para"></p>
```

Example:

```html
<p class="note">Important Note</p>
```

---

## style

### Definition

The `style` attribute is used to apply inline CSS to an element.

### Syntax

```html
<p style="color:red;">
```

Example:

```html
<h1 style="color:blue;">
Welcome
</h1>
```

---

## title

### Definition

The `title` attribute displays extra information as a tooltip when the user moves the mouse over the element.

### Syntax

```html
<p title="Information">
```

Example:

```html
<p title="This is HTML5">
Move Mouse Here
</p>
```

---

## lang

### Definition

The `lang` attribute specifies the language of the webpage.

### Syntax

```html
<html lang="en">
```

Example:

```html
<html lang="en">
```

Here:

```text
en = English
```

---

## hidden

### Definition

The `hidden` attribute hides an element from the browser.

### Syntax

```html
<p hidden>
```

Example:

```html
<p hidden>
This content is hidden.
</p>
```

---

# 2. Anchor `<a>` Attributes

The `<a>` tag is used to create hyperlinks.

---

## href

### Definition

The `href` attribute specifies the destination URL.

### Syntax

```html
<a href="URL">
```

Example:

```html
<a href="https://www.google.com">
Google
</a>
```

---

## target

### Definition

The `target` attribute specifies where the linked document should open.

### Common Values

| Value  | Meaning  |
| ------ | -------- |
| _self  | Same tab |
| _blank | New tab  |

Example:

```html
<a href="https://www.google.com"
   target="_blank">
Google
</a>
```

---

## download

### Definition

The `download` attribute tells the browser to download the linked file.

Example:

```html
<a href="resume.pdf" download>
Download Resume
</a>
```

---

## rel

### Definition

The `rel` attribute defines the relationship between the current page and linked page.

Example:

```html
<a href="https://example.com"
target="_blank"
rel="noopener">
```

---

# 3. Image `<img>` Attributes

---

## src

### Definition

The `src` attribute specifies the image path.

Example:

```html
<img src="image.jpg">
```

---

## alt

### Definition

The `alt` attribute provides alternate text if the image cannot load.

Example:

```html
<img src="java.png"
alt="Java Logo">
```

---

## width

### Definition

Specifies image width.

Example:

```html
<img src="java.png"
width="200">
```

---

## height

### Definition

Specifies image height.

Example:

```html
<img src="java.png"
height="150">
```

---

## loading

### Definition

Controls image loading behavior.

Example:

```html
<img src="image.jpg"
loading="lazy">
```

### Types

```text
lazy  -> Load when needed
eager -> Load immediately
```

---

# 4. Audio `<audio>` Attributes

---

## controls

Adds:

* Play Button
* Pause Button
* Volume Control

Example:

```html
<audio controls>
```

---

## src

Specifies audio file.

Example:

```html
<audio src="song.mp3">
```

---

## autoplay

Starts audio automatically.

Example:

```html
<audio autoplay>
```

---

## loop

Repeats audio continuously.

Example:

```html
<audio loop>
```

---

## muted

Starts audio in mute mode.

Example:

```html
<audio muted>
```

---

# 5. Video `<video>` Attributes

---

## controls

Displays video controls.

Example:

```html
<video controls>
```

---

## src

Specifies video path.

Example:

```html
<video src="movie.mp4">
```

---

## width

Specifies video width.

Example:

```html
width="320"
```

---

## height

Specifies video height.

Example:

```html
height="240"
```

---

## autoplay

Automatically plays video.

Example:

```html
<video autoplay>
```

---

## loop

Repeats video.

Example:

```html
<video loop>
```

---

## poster

Displays an image before video starts.

Example:

```html
<video poster="cover.jpg">
```

---

## muted

Starts video silently.

Example:

```html
<video muted>
```

---

# 6. Table Attributes

---

## border

### Definition

Adds borders to the table.

Example:

```html
<table border="1">
```

---

## colspan

### Definition

Allows a cell to occupy multiple columns.

Example:

```html
<td colspan="2">
```

---

## rowspan

### Definition

Allows a cell to occupy multiple rows.

Example:

```html
<td rowspan="3">
```

---

# 7. Form Attributes

---

## action

Specifies where form data should be sent.

Example:

```html
<form action="save.java">
```

---

## method

Specifies HTTP request type.

### Types

```text
GET
POST
```

Example:

```html
<form method="POST">
```

---

## enctype

Specifies data encoding.

Example:

```html
<form enctype="multipart/form-data">
```

Used for:

* File Uploads

---

## autocomplete

Allows browser auto-fill.

Example:

```html
<form autocomplete="on">
```

---

# 8. Input Attributes

---

## type

Specifies input type.

Example:

```html
<input type="text">
```

Common Types:

```text
text
password
email
number
radio
checkbox
submit
date
file
```

---

## name

Specifies the variable name sent to server.

Example:

```html
<input name="username">
```

---

## value

Specifies default value.

Example:

```html
<input value="Java">
```

---

## placeholder

Displays sample input text.

Example:

```html
<input placeholder="Enter Name">
```

---

## required

Makes the field mandatory.

Example:

```html
<input required>
```

---

## pattern

Validates input using Regular Expressions.

Example:

```html
<input pattern="[0-9]{10}">
```

---

## readonly

Makes input read-only.

Example:

```html
<input readonly>
```

---

## disabled

Disables the input field.

Example:

```html
<input disabled>
```

---

# 9. Label Attribute

## for

### Definition

Associates a label with an input element.

### Example

```html
<label for="username">
Username
</label>

<input id="username">
```

Clicking the label automatically focuses the input field.

---

# 10. Option Attributes

---

## value

Specifies the value submitted to the server.

Example:

```html
<option value="Java">
Java
</option>
```

---

## selected

Makes an option selected by default.

Example:

```html
<option selected>
Java
</option>
```

---

# Important Points

* Attributes provide additional information about elements.
* Attributes are written inside the opening tag.
* Most attributes use:

```html
attribute="value"
```

* Global attributes can be used with most HTML elements.
* Form attributes control form submission behavior.
* Input attributes provide validation and user interaction.
* Media attributes control audio and video behavior.

---

# Summary

HTML5 Attributes provide additional functionality and control over HTML elements. Attributes such as `id`, `class`, `href`, `src`, `action`, `method`, `placeholder`, `required`, and `pattern` are among the most frequently used attributes in modern web development. Understanding these attributes is essential for creating interactive, responsive, and professional web applications.
