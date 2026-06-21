# 03 - Heading Tags in HTML

## Introduction

Heading tags are used to define headings and subheadings in an HTML document.

HTML provides six levels of headings:

* `<h1>` to `<h6>`
* `<h1>` is the largest and most important heading.
* `<h6>` is the smallest heading.

---

## Example Program

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Heading Tags</title>
</head>
<body>
    <h1>Heading 1 Tag</h1>
    <h2>Heading 2 Tag</h2>
    <h3>Heading 3 Tag</h3>
    <h4>Heading 4 Tag</h4>
    <h5>Heading 5 Tag</h5>
    <h6>Heading 6 Tag</h6>
</body>
</html>
```

---

## Heading Tags Used

### 1. `<h1></h1>`

#### Definition

The `<h1>` tag defines the most important heading on a webpage.

#### Features

* Largest heading tag.
* Highest importance for SEO.
* Usually used for the main title of the webpage.

#### Example

```html
<h1>Welcome to HTML</h1>
```

Output:

```text
Welcome to HTML
```

---

### 2. `<h2></h2>`

#### Definition

The `<h2>` tag defines a second-level heading.

#### Features

* Smaller than `<h1>`.
* Used for major sections of a webpage.

#### Example

```html
<h2>Introduction</h2>
```

---

### 3. `<h3></h3>`

#### Definition

The `<h3>` tag defines a third-level heading.

#### Features

* Used for sub-sections inside an `<h2>` section.

#### Example

```html
<h3>Features of HTML</h3>
```

---

### 4. `<h4></h4>`

#### Definition

The `<h4>` tag defines a fourth-level heading.

#### Features

* Used for smaller sub-sections.

#### Example

```html
<h4>HTML Elements</h4>
```

---

### 5. `<h5></h5>`

#### Definition

The `<h5>` tag defines a fifth-level heading.

#### Features

* Smaller than `<h4>`.
* Used for less important headings.

#### Example

```html
<h5>Additional Information</h5>
```

---

### 6. `<h6></h6>`

#### Definition

The `<h6>` tag defines the smallest heading.

#### Features

* Smallest heading available in HTML.
* Used for minor headings or notes.

#### Example

```html
<h6>Footer Information</h6>
```

---

## Output of the Program

```text
Heading 1 Tag

Heading 2 Tag

Heading 3 Tag

Heading 4 Tag

Heading 5 Tag

Heading 6 Tag
```

The size of the headings decreases from `<h1>` to `<h6>`.

---

## Difference Between Heading Tags

| Tag | Size         | Importance |
| --- | ------------ | ---------- |
| h1  | Largest      | Highest    |
| h2  | Large        | High       |
| h3  | Medium Large | Moderate   |
| h4  | Medium       | Less       |
| h5  | Small        | Low        |
| h6  | Smallest     | Lowest     |

---

## Important Points

* HTML provides six heading tags from `<h1>` to `<h6>`.
* `<h1>` should generally be used only once on a webpage.
* Heading tags improve the structure and readability of a webpage.
* Search engines use heading tags to understand webpage content.
* Proper use of heading tags improves SEO (Search Engine Optimization).

---

## Summary

Heading tags are used to create titles and subheadings in an HTML document. They help organize content, improve readability, and play an important role in Search Engine Optimization (SEO). The `<h1>` tag represents the most important heading, while `<h6>` represents the least important heading.
