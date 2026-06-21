# 05 - Hyperlinks and Media Tags in HTML

## Introduction

HTML provides special tags to create hyperlinks and embed multimedia content such as images, audio, and videos into a web page.

These tags help developers create interactive and visually appealing websites.

The important tags covered in this file are:

* `<a>` - Hyperlink Tag
* `<img>` - Image Tag
* `<audio>` - Audio Tag
* `<video>` - Video Tag
* `<source>` - Media Source Tag

---

## Example Program

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Hyperlinks and Media Tags</title>
</head>
<body>

    <h2>1. Navigation Links</h2>

    <p>
        Visit the official
        <a href="https://www.google.com" target="_blank">
            Google Search Engine
        </a>
        in a new tab.
    </p>

    <h2>2. Embedded Graphics</h2>

    <img src="https://via.placeholder.com/150"
         width="150"
         height="150"
         alt="Sample Image">

    <h2>3. Native Audio Streaming</h2>

    <audio controls>
        <source src="podcast.mp3" type="audio/mpeg">
    </audio>

    <h2>4. Native Video Playback</h2>

    <video controls width="320" height="240">
        <source src="movie.mp4" type="video/mp4">
    </video>

</body>
</html>
```

---

## 1. `<a>` - Hyperlink Tag

### Definition

The `<a>` tag is called the **Anchor Tag**.

It is used to create hyperlinks that allow users to navigate from one webpage to another webpage or website.

### Syntax

```html
<a href="URL">Link Text</a>
```

### Example

```html
<a href="https://www.google.com">
Google Search Engine
</a>
```

### Attributes

#### href

Specifies the destination URL.

Example:

```html
href="https://www.google.com"
```

#### target

Specifies where the linked page should open.

Example:

```html
target="_blank"
```

`_blank` opens the page in a new browser tab.

---

## 2. `<img>` - Image Tag

### Definition

The `<img>` tag is used to display images on a webpage.

It is an **unpaired tag**, which means it does not require a closing tag.

### Syntax

```html
<img src="image.jpg">
```

### Example

```html
<img src="https://via.placeholder.com/150"
     width="150"
     height="150">
```

### Important Attributes

#### src

Specifies the image location.

#### width

Defines the width of the image.

#### height

Defines the height of the image.

#### alt

Provides alternate text when the image cannot be loaded.

Example:

```html
alt="Sample Image"
```

---

## 3. `<audio>` - Audio Tag

### Definition

The `<audio>` tag is used to embed audio files into a webpage.

HTML5 supports audio playback without requiring external plugins.

### Syntax

```html
<audio controls>

</audio>
```

### Example

```html
<audio controls>
    <source src="podcast.mp3"
            type="audio/mpeg">
</audio>
```

### Attribute

#### controls

Displays:

* Play button
* Pause button
* Volume controls
* Progress bar

---

## 4. `<video>` - Video Tag

### Definition

The `<video>` tag is used to embed video files into a webpage.

HTML5 allows videos to play directly in browsers.

### Syntax

```html
<video controls>

</video>
```

### Example

```html
<video controls
       width="320"
       height="240">

    <source src="movie.mp4"
            type="video/mp4">

</video>
```

### Attributes

#### controls

Displays video controls.

#### width

Sets video width.

#### height

Sets video height.

---

## 5. `<source>` - Source Tag

### Definition

The `<source>` tag specifies media files for:

* Audio
* Video

It allows browsers to choose a compatible media format.

### Syntax

```html
<source src="file.mp3"
        type="audio/mpeg">
```

### Example

```html
<source src="movie.mp4"
        type="video/mp4">
```

---

## Explanation of the Program

### Title Tag

```html
<title>Hyperlinks and Media Tags</title>
```

Displays the title on the browser tab.

---

### Hyperlink

```html
<a href="https://www.google.com"
target="_blank">
Google Search Engine
</a>
```

Creates a clickable hyperlink that opens Google in a new tab.

---

### Image

```html
<img src="https://via.placeholder.com/150"
width="150"
height="150">
```

Displays an image with width and height of 150 pixels.

---

### Audio

```html
<audio controls>
```

Creates an audio player with playback controls.

---

### Video

```html
<video controls width="320" height="240">
```

Creates a video player with playback controls.

---

## Important Points

* `<a>` is used to create hyperlinks.
* `<img>` is used to display images.
* `<img>` is an unpaired tag.
* `<audio>` is used for audio playback.
* `<video>` is used for video playback.
* `<source>` specifies media files.
* `target="_blank"` opens a link in a new tab.
* HTML5 multimedia does not require external plugins.

---

## Summary

Hyperlinks and Media Tags are essential elements of modern HTML5 web development. The `<a>` tag enables website navigation, while `<img>`, `<audio>`, and `<video>` allow developers to create interactive and multimedia-rich webpages. These tags are fundamental concepts for Front-end Development and Java Full Stack Development.
