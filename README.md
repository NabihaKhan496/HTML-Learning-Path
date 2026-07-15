# 🌐 HTML Learning Path

Welcome to **HTML Learning Path**!

This repository is made for beginners who want to learn HTML from scratch. Every HTML tag is explained in **simple language** with a short description, a one-line example, and easy-to-understand explanations.

Whether you are a student, a beginner, or someone preparing for interviews, this guide will help you understand HTML step by step.

Each HTML tag includes:
- 📖 A simple explanation
- 💡 A one-line example
- 📝 Easy-to-understand descriptions
- 🚀 Beginner-friendly language

---

> 💡 **How to use this guide:**  
> Start from **Chapter 1** and continue in order, or use the **Table of Contents** below to jump directly to any topic.

---

# 📑 Table of Contents

1. [Document Structure](#1-document-structure)
2. [Metadata & Head Elements](#2-metadata--head-elements)
3. [Headings & Text Content](#3-headings--text-content)
4. [Text Formatting & Inline Semantics](#4-text-formatting--inline-semantics)
5. [Lists](#5-lists)
6. [Links & Navigation](#6-links--navigation)
7. [Images & Media](#7-images--media)
8. [Tables](#8-tables)
9. [Forms & Input](#9-forms--input)
10. [Semantic Layout (HTML5)](#10-semantic-layout-html5)
11. [Scripting & Templates](#11-scripting--templates)
12. [Interactive & Miscellaneous](#12-interactive--miscellaneous)
13. [Deprecated Tags (Good to Recognize, Avoid Using)](#13-deprecated-tags-good-to-recognize-avoid-using)

Happy Learning! 🚀

---

# 1. Document Structure

Every HTML page starts with a basic structure. These elements tell the browser that the file is an HTML document and organize the webpage into different parts.

---

## `<!DOCTYPE html>`

### Description

`<!DOCTYPE html>` tells the browser that the document is written in **HTML5**. It should always be the **first line** of every HTML document.

### Example

```html
<!DOCTYPE html>
```

### Explanation

Without this declaration, the browser may not display the webpage correctly.

---

## `<html>`

### Description

The `<html>` tag is the **root element** of an HTML page. Every other HTML element is written inside this tag.

### Example

```html
<html lang="en"></html>
```

### Explanation

The `lang="en"` attribute tells browsers and screen readers that the page language is English.

---

## `<head>`

### Description

The `<head>` tag contains information **about the webpage**, not the visible content. It usually includes the page title, metadata, CSS, and links to external files.

### Example

```html
<head></head>
```

### Explanation

Anything inside the `<head>` tag is **not displayed** on the webpage.

---

## `<body>`

### Description

The `<body>` tag contains everything that is **visible** on the webpage, such as headings, paragraphs, images, tables, forms, buttons, and more.

### Example

```html
<body>Hello, World!</body>
```

### Explanation

Everything that users see in the browser is written inside the `<body>` tag.

---

## Complete Example

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>My First Web Page</title>
</head>

<body>
    <h1>Welcome to HTML</h1>
    <p>This is my first HTML page.</p>
</body>

</html>
```

### Output

```
Welcome to HTML

This is my first HTML page.
```

---

### 📌 Summary

| Tag | Purpose |
|------|---------|
| `<!DOCTYPE html>` | Declares that the document uses HTML5. |
| `<html>` | The root element that contains the entire webpage. |
| `<head>` | Stores page information such as the title and metadata. |
| `<body>` | Contains all the visible content shown in the browser. |

---

---

# 2. Metadata & Head Elements

Metadata elements provide information **about the webpage**. They are placed inside the `<head>` tag and help browsers, search engines, and other tools understand your webpage.

---

## `<title>`

### Description

The `<title>` tag defines the title of a webpage. The title appears in the browser tab and is also used by search engines.

### Why We Use It

- Displays the page title in the browser tab.
- Helps search engines identify the webpage.
- Makes bookmarks easier to recognize.

### Example

```html
<title>My First Website</title>
```

### Explanation

When you open the webpage, **"My First Website"** appears on the browser tab.

---

## `<meta>`

### Description

The `<meta>` tag provides additional information (metadata) about the webpage. It is not visible on the page.

### Why We Use It

- Defines the character encoding.
- Makes the page responsive on all devices.
- Provides information for search engines.

### Example

```html
<meta charset="UTF-8">
```

### Explanation

This tells the browser to use the **UTF-8** character encoding, which supports most languages and special characters.

---

## `<link>`

### Description

The `<link>` tag connects external files to the HTML document. It is most commonly used to attach CSS files or a favicon.

### Why We Use It

- Connect external CSS files.
- Add a website icon (favicon).
- Improve code organization.

### Example

```html
<link rel="stylesheet" href="style.css">
```

### Explanation

This line connects the external CSS file named **style.css** to the webpage.

---

## `<style>`

### Description

The `<style>` tag is used to write CSS directly inside the HTML document.

### Why We Use It

- Add CSS without creating a separate file.
- Style a single webpage.
- Test CSS quickly.

### Example

```html
<style>body { background-color: lightblue; }</style>
```

### Explanation

This changes the background color of the webpage to **light blue**.

---

## `<base>`

### Description

The `<base>` tag sets a default URL or default target for all links on the webpage.

### Why We Use It

- Set a common base URL for links.
- Make all links open in the same target window.
- Reduce repetitive code.

### Example

```html
<base href="https://example.com/" target="_blank">
```

### Explanation

All relative links on the page will use **https://example.com/** as their starting location and open in a new tab.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<title>` | Sets the title shown in the browser tab. |
| `<meta>` | Provides metadata about the webpage. |
| `<link>` | Connects external resources like CSS files. |
| `<style>` | Adds internal CSS styles. |
| `<base>` | Sets the default URL and target for links. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
