# 06 - Lists in HTML

## Introduction

HTML provides different types of lists to organize and display related information in a structured manner.

There are three types of lists in HTML:

1. Ordered List (`<ol>`)
2. Unordered List (`<ul>`)
3. Description List (`<dl>`)

Lists improve readability and help present information in a clear and organized format.

---

## Example Program

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>List and Description List Tags</title>
</head>
<body>

<fieldset>

    <h2>1. Ordered List (Sequential Steps)</h2>

    <p>How to execute a database operation:</p>

    <ol>
        <li>Establish database connection</li>
        <li>Compile the SQL query statement</li>
        <li>Execute update and close connection blocks</li>
    </ol>

</fieldset>

<br>

<fieldset>

    <h2>2. Unordered List (Core Technologies)</h2>

    <p>Essential components of front-end engineering:</p>

    <ul>
        <li>HTML5</li>
        <li>CSS3</li>
        <li>JavaScript</li>
    </ul>

</fieldset>

<br>

<fieldset>

    <h2>3. Description List (Glossary Definition Layout)</h2>

    <p>Web Architecture Key Terms:</p>

    <dl>

        <dt>HTML</dt>

        <dd>
            A structural markup language used to build the content backbone of web documents.
        </dd>

        <dt>CSS</dt>

        <dd>
            A design sheets engine used to handle the layout, formatting, and skin aesthetics of web pages.
        </dd>

    </dl>

</fieldset>

</body>
</html>
```

---

## 1. Ordered List (`<ol>`)

### Definition

The `<ol>` tag stands for **Ordered List**.

It is used when items should appear in a specific order or sequence.

By default, browsers display ordered lists with numbers.

### Syntax

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
</ol>
```

### Example

```html
<ol>
    <li>Establish database connection</li>
    <li>Compile SQL query</li>
    <li>Execute query</li>
</ol>
```

### Output

```text
1. Establish database connection
2. Compile SQL query
3. Execute query
```

---

## 2. List Item Tag (`<li>`)

### Definition

The `<li>` tag stands for **List Item**.

It is used to define an item inside:

* Ordered Lists (`<ol>`)
* Unordered Lists (`<ul>`)

### Syntax

```html
<li>HTML5</li>
```

### Example

```html
<li>JavaScript</li>
```

Output:

```text
• JavaScript
```

---

## 3. Unordered List (`<ul>`)

### Definition

The `<ul>` tag stands for **Unordered List**.

It is used when the order of items is not important.

By default, browsers display bullet points.

### Syntax

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>
```

### Example

```html
<ul>
    <li>HTML5</li>
    <li>CSS3</li>
    <li>JavaScript</li>
</ul>
```

### Output

```text
• HTML5
• CSS3
• JavaScript
```

---

## 4. Description List (`<dl>`)

### Definition

The `<dl>` tag stands for **Description List**.

It is used to create a list of terms along with their descriptions.

### Syntax

```html
<dl>

</dl>
```

Inside `<dl>`, we use:

* `<dt>` → Description Term
* `<dd>` → Description Definition

---

## 5. Description Term (`<dt>`)

### Definition

The `<dt>` tag stands for **Description Term**.

It defines the term or title.

### Example

```html
<dt>HTML</dt>
```

Output:

```text
HTML
```

---

## 6. Description Definition (`<dd>`)

### Definition

The `<dd>` tag stands for **Description Definition**.

It provides the explanation of the term defined in `<dt>`.

### Example

```html
<dd>
A structural markup language used to build web pages.
</dd>
```

---

## 7. Fieldset Tag (`<fieldset>`)

### Definition

The `<fieldset>` tag is used to group related elements inside a box.

It creates a visible border around content.

### Syntax

```html
<fieldset>

Content

</fieldset>
```

### Example

```html
<fieldset>

<h2>Ordered List</h2>

<ol>
    <li>Step 1</li>
    <li>Step 2</li>
</ol>

</fieldset>
```

---

## Explanation of the Program

### Ordered List Section

```html
<ol>
```

Creates a numbered list.

```html
<li>
```

Represents each list item.

---

### Unordered List Section

```html
<ul>
```

Creates a bulleted list.

```html
<li>
```

Represents each bullet item.

---

### Description List Section

```html
<dl>
```

Creates a description list.

```html
<dt>
```

Defines the term.

```html
<dd>
```

Defines the description of that term.

---

## Difference Between Lists

| List Type        | Tag    | Output                 |
| ---------------- | ------ | ---------------------- |
| Ordered List     | `<ol>` | Numbers                |
| Unordered List   | `<ul>` | Bullets                |
| Description List | `<dl>` | Terms with Definitions |

---

## Important Points

* `<ol>` creates numbered lists.
* `<ul>` creates bulleted lists.
* `<li>` defines list items.
* `<dl>` creates description lists.
* `<dt>` defines terms.
* `<dd>` defines descriptions.
* `<fieldset>` groups related content with a border.
* Lists are widely used in menus, navigation bars, forms, and documentation.

---

## Summary

HTML Lists are used to organize information in a structured and readable format. Ordered Lists display numbered items, Unordered Lists display bullet points, and Description Lists provide terms with explanations. Lists are one of the most frequently used elements in modern web development and are essential concepts for every Front-end Developer and Java Full Stack Developer.
