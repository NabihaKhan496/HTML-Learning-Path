# 🌐 HTML Reference Guide

Welcome to **HTML Reference Guide**!

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
> 💻 **index.html** — A complete sample webpage built using the HTML elements explained in this guide. You can open it in your browser or inspect the source code to see how each element is used in practice.
Read each chapter in this README, then open **index.html** and find the corresponding HTML element in the code. Make small changes, save the file, and refresh your browser to see the results. Hands-on practice is one of the best ways to learn HTML.

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
---

# 3. Headings & Text Content

Text content elements are used to display headings, paragraphs, line breaks, horizontal lines, and organize text on a webpage.

---

## `<h1>` to `<h6>`

### Description

The `<h1>` to `<h6>` tags are used to create headings. `<h1>` is the largest and most important heading, while `<h6>` is the smallest.

### Why We Use It

- Create titles and subtitles.
- Organize webpage content.
- Improve readability.
- Help search engines understand the page structure.

### Example

```html
<h1>Welcome to HTML</h1>
```

### Explanation

This displays **"Welcome to HTML"** as the main heading of the webpage.

> **Note:** Use only one `<h1>` tag for the main title of a webpage whenever possible.

---

## `<p>`

### Description

The `<p>` tag is used to create a paragraph.

### Why We Use It

- Display normal text.
- Write descriptions.
- Create readable content.

### Example

```html
<p>HTML is the standard markup language for creating web pages.</p>
```

### Explanation

This displays a paragraph containing the given text.

---

## `<br>`

### Description

The `<br>` tag inserts a single line break.

### Why We Use It

- Move text to the next line.
- Write addresses.
- Display poems or song lyrics.

### Example

```html
First Line<br>Second Line
```

### Explanation

The second line starts immediately below the first line without creating a new paragraph.

---

## `<hr>`

### Description

The `<hr>` tag creates a horizontal line to separate different sections of content.

### Why We Use It

- Divide sections.
- Improve page organization.
- Create visual separation.

### Example

```html
<hr>
```

### Explanation

A horizontal line appears across the webpage.

---

## `<div>`

### Description

The `<div>` tag is a block-level container used to group other HTML elements.

### Why We Use It

- Group related content.
- Apply CSS styles.
- Create webpage layouts.

### Example

```html
<div>This is a container.</div>
```

### Explanation

The text is placed inside a separate block that can be styled or organized using CSS.

---

## `<span>`

### Description

The `<span>` tag is an inline container used to style or group a small part of text.

### Why We Use It

- Style specific words.
- Apply CSS to part of a sentence.
- Group inline elements.

### Example

```html
<span>Hello</span>
```

### Explanation

The word **Hello** is wrapped inside a `<span>` without starting a new line.

---

## `<pre>`

### Description

The `<pre>` tag displays text exactly as it is written, including spaces and line breaks.

### Why We Use It

- Display code.
- Preserve formatting.
- Show text with fixed spacing.

### Example

```html
<pre>Hello
World</pre>
```

### Explanation

The browser displays the text with the same spaces and line breaks as written.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<h1>`–`<h6>` | Creates headings of different sizes. |
| `<p>` | Creates a paragraph. |
| `<br>` | Inserts a line break. |
| `<hr>` | Creates a horizontal line. |
| `<div>` | Groups block-level elements. |
| `<span>` | Groups inline text or elements. |
| `<pre>` | Displays preformatted text while preserving spaces and line breaks. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 4. Text Formatting & Inline Semantics

Text formatting tags are used to change the appearance or meaning of text. Some tags only change how the text looks, while others also tell browsers and search engines that the text has a special meaning.

---

## `<strong>`

### Description

The `<strong>` tag is used to show that a piece of text is **very important**. Browsers usually display it in **bold**.

### Why We Use It

- Highlight important information.
- Improve accessibility.
- Indicate strong importance.

### Syntax

```html
<strong>Important Text</strong>
```

### Example

```html
<strong>Warning!</strong>
```

### Explanation

The word **Warning!** appears in bold and tells readers that it is important.

---

## `<b>`

### Description

The `<b>` tag makes text **bold** without adding any special meaning.

### Why We Use It

- Make text stand out.
- Draw the reader's attention.
- Style text visually.

### Syntax

```html
<b>Bold Text</b>
```

### Example

```html
<b>HTML</b>
```

### Explanation

The word **HTML** appears in bold, but it does not indicate importance.

---

## `<em>`

### Description

The `<em>` tag is used to emphasize text. Browsers usually display it in *italic*.

### Why We Use It

- Emphasize important words.
- Improve readability.
- Add semantic meaning.

### Syntax

```html
<em>Emphasized Text</em>
```

### Example

```html
<em>Please read carefully.</em>
```

### Explanation

The sentence appears in italic and indicates emphasis.

---

## `<i>`

### Description

The `<i>` tag displays text in *italic* for styling purposes only.

### Why We Use It

- Display foreign words.
- Display book titles.
- Style text.

### Syntax

```html
<i>Italic Text</i>
```

### Example

```html
<i>Bonjour</i>
```

### Explanation

The word **Bonjour** appears in italic without adding semantic importance.

---

## `<mark>`

### Description

The `<mark>` tag highlights text.

### Why We Use It

- Highlight search results.
- Draw attention to important text.

### Syntax

```html
<mark>Highlighted Text</mark>
```

### Example

```html
<mark>HTML</mark>
```

### Explanation

The word **HTML** appears highlighted with a yellow background.

---

## `<small>`

### Description

The `<small>` tag displays text in a smaller font size.

### Why We Use It

- Display copyright text.
- Show notes or comments.
- Display additional information.

### Syntax

```html
<small>Small Text</small>
```

### Example

```html
<small>© 2026 HTML Reference Guide</small>
```

### Explanation

The copyright text appears smaller than normal text.

---

## `<del>`

### Description

The `<del>` tag represents deleted text. Browsers usually display it with a strikethrough.

### Why We Use It

- Show removed content.
- Compare old and new information.

### Syntax

```html
<del>Old Text</del>
```

### Example

```html
<del>$100</del>
```

### Explanation

The old price appears with a line through it.

---

## `<ins>`

### Description

The `<ins>` tag represents newly inserted text. Browsers usually underline it.

### Why We Use It

- Show added information.
- Highlight updated content.

### Syntax

```html
<ins>New Text</ins>
```

### Example

```html
<ins>$80</ins>
```

### Explanation

The new price appears underlined.

---

## `<sub>`

### Description

The `<sub>` tag displays text as subscript.

### Why We Use It

- Write chemical formulas.
- Display mathematical expressions.

### Syntax

```html
<sub>Subscript</sub>
```

### Example

```html
H<sub>2</sub>O
```

### Explanation

The number **2** appears below the normal text.

---

## `<sup>`

### Description

The `<sup>` tag displays text as superscript.

### Why We Use It

- Write exponents.
- Display footnotes.

### Syntax

```html
<sup>Superscript</sup>
```

### Example

```html
x<sup>2</sup>
```

### Explanation

The number **2** appears above the normal text.

---

## `<code>`

### Description

The `<code>` tag is used to display computer code.

### Why We Use It

- Show programming code.
- Display commands.
- Display function names.

### Syntax

```html
<code>Code</code>
```

### Example

```html
<code>console.log()</code>
```

### Explanation

The code appears in a monospace font.

---

## `<kbd>`

### Description

The `<kbd>` tag represents keyboard input.

### Why We Use It

- Show keyboard shortcuts.
- Display keyboard keys.

### Syntax

```html
<kbd>Key</kbd>
```

### Example

```html
<kbd>Ctrl + C</kbd>
```

### Explanation

This represents the keyboard shortcut **Ctrl + C**.

---

## `<samp>`

### Description

The `<samp>` tag displays sample output from a computer program.

### Why We Use It

- Show program output.
- Display console results.

### Syntax

```html
<samp>Output</samp>
```

### Example

```html
<samp>Hello World</samp>
```

### Explanation

This represents the output produced by a program.

---

## `<var>`

### Description

The `<var>` tag represents a variable in programming or mathematics.

### Why We Use It

- Display variable names.
- Show mathematical variables.

### Syntax

```html
<var>Variable</var>
```

### Example

```html
<var>x</var>
```

### Explanation

The letter **x** represents a variable.

---

## `<abbr>`

### Description

The `<abbr>` tag defines an abbreviation or acronym.

### Why We Use It

- Explain abbreviations.
- Improve accessibility.

### Syntax

```html
<abbr title="Full Meaning">Short Form</abbr>
```

### Example

```html
<abbr title="HyperText Markup Language">HTML</abbr>
```

### Explanation

When the user hovers over **HTML**, the full meaning appears as a tooltip.

---

## `<cite>`

### Description

The `<cite>` tag is used for the title of a book, movie, song, or other creative work.

### Why We Use It

- Reference creative works.
- Display titles correctly.

### Syntax

```html
<cite>Title</cite>
```

### Example

```html
<cite>Harry Potter</cite>
```

### Explanation

The book title is displayed in italic by most browsers.

---

## `<blockquote>`

### Description

The `<blockquote>` tag is used for long quotations from another source.

### Why We Use It

- Display long quotes.
- Credit another source.

### Syntax

```html
<blockquote>Quote</blockquote>
```

### Example

```html
<blockquote>Learning never stops.</blockquote>
```

### Explanation

The quotation is displayed as a separate block.

---

## `<q>`

### Description

The `<q>` tag is used for short inline quotations.

### Why We Use It

- Quote short sentences.
- Add quotation marks automatically.

### Syntax

```html
<q>Quote</q>
```

### Example

```html
<q>Practice makes perfect.</q>
```

### Explanation

The browser automatically adds quotation marks around the text.

---

## `<address>`

### Description

The `<address>` tag contains contact information.

### Why We Use It

- Display contact details.
- Show author information.

### Syntax

```html
<address>Contact Information</address>
```

### Example

```html
<address>Email: info@example.com</address>
```

### Explanation

Displays contact information for the website or author.

---

## `<time>`

### Description

The `<time>` tag represents a specific date or time.

### Why We Use It

- Display dates.
- Display time.
- Improve machine readability.

### Syntax

```html
<time datetime="2026-07-15">July 15, 2026</time>
```

### Example

```html
<time datetime="09:00">9:00 AM</time>
```

### Explanation

Displays the time while providing a machine-readable value.

---

## `<wbr>`

### Description

The `<wbr>` tag suggests a place where a long word can break into the next line if needed.

### Why We Use It

- Prevent layout issues.
- Improve readability of long words or URLs.

### Syntax

```html
LongWord<wbr>AnotherWord
```

### Example

```html
supercalifragilistic<wbr>expialidocious
```

### Explanation

The browser may break the word at the `<wbr>` position if there is not enough space.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<strong>` | Indicates important text. |
| `<b>` | Makes text bold. |
| `<em>` | Emphasizes text. |
| `<i>` | Displays italic text. |
| `<mark>` | Highlights text. |
| `<small>` | Displays smaller text. |
| `<del>` | Shows deleted text. |
| `<ins>` | Shows inserted text. |
| `<sub>` | Displays subscript text. |
| `<sup>` | Displays superscript text. |
| `<code>` | Displays computer code. |
| `<kbd>` | Represents keyboard input. |
| `<samp>` | Displays sample program output. |
| `<var>` | Represents a variable. |
| `<abbr>` | Defines an abbreviation. |
| `<cite>` | References a creative work. |
| `<blockquote>` | Displays a long quotation. |
| `<q>` | Displays a short quotation. |
| `<address>` | Displays contact information. |
| `<time>` | Represents a date or time. |
| `<wbr>` | Suggests a word break location. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 5. Lists

Lists are used to organize information in a structured way. HTML provides three types of lists:

- **Unordered List** (Bulleted List)
- **Ordered List** (Numbered List)
- **Description List** (Term and Description)

---

## `<ul>` (Unordered List)

### Description

The `<ul>` tag creates an **unordered list**. Items in the list are displayed with bullet points by default.

### Why We Use It

- Create bulleted lists.
- Display items where the order does not matter.
- Organize related information.

### Syntax

```html
<ul>
    <li>Item</li>
</ul>
```

### Example

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### Explanation

This displays a bulleted list containing HTML, CSS, and JavaScript.

---

## `<ol>` (Ordered List)

### Description

The `<ol>` tag creates an **ordered list**. Items are displayed with numbers by default.

### Why We Use It

- Show steps in order.
- Display rankings.
- Create numbered lists.

### Syntax

```html
<ol>
    <li>Item</li>
</ol>
```

### Example

```html
<ol>
    <li>Wake Up</li>
    <li>Study HTML</li>
    <li>Practice Coding</li>
</ol>
```

### Explanation

This displays a numbered list from 1 to 3.

---

## `<li>` (List Item)

### Description

The `<li>` tag represents a single item inside an ordered or unordered list.

### Why We Use It

- Add items to a list.
- Organize list content.

### Syntax

```html
<li>List Item</li>
```

### Example

```html
<li>HTML</li>
```

### Explanation

This creates one item inside a list. The `<li>` tag must be placed inside either a `<ul>` or an `<ol>` tag.

---

## `<dl>` (Description List)

### Description

The `<dl>` tag creates a **description list**. It is used to display terms along with their descriptions.

### Why We Use It

- Define words.
- Create glossaries.
- Display questions and answers.

### Syntax

```html
<dl>
    <dt>Term</dt>
    <dd>Description</dd>
</dl>
```

### Example

```html
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
</dl>
```

### Explanation

This displays **HTML** as the term and **HyperText Markup Language** as its description.

---

## `<dt>` (Description Term)

### Description

The `<dt>` tag defines the **term or title** in a description list.

### Why We Use It

- Display the name of a term.
- Define a word before its description.

### Syntax

```html
<dt>Term</dt>
```

### Example

```html
<dt>CSS</dt>
```

### Explanation

This represents the term **CSS** inside a description list.

---

## `<dd>` (Description Details)

### Description

The `<dd>` tag provides the **description or definition** of a term in a description list.

### Why We Use It

- Explain a term.
- Provide additional information.

### Syntax

```html
<dd>Description</dd>
```

### Example

```html
<dd>Cascading Style Sheets</dd>
```

### Explanation

This provides the description of the term **CSS**.

---

## Complete Example

```html
<h3>Unordered List</h3>

<ul>
    <li>Apple</li>
    <li>Mango</li>
    <li>Orange</li>
</ul>

<h3>Ordered List</h3>

<ol>
    <li>Register</li>
    <li>Login</li>
    <li>Start Learning</li>
</ol>

<h3>Description List</h3>

<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>

    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>
</dl>
```

### Output

**Unordered List**

- Apple
- Mango
- Orange

**Ordered List**

1. Register
2. Login
3. Start Learning

**Description List**

**HTML**  
HyperText Markup Language

**CSS**  
Cascading Style Sheets

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<ul>` | Creates a bulleted (unordered) list. |
| `<ol>` | Creates a numbered (ordered) list. |
| `<li>` | Defines a list item. |
| `<dl>` | Creates a description list. |
| `<dt>` | Defines the term in a description list. |
| `<dd>` | Defines the description of a term. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)
---
---

# 6. Links & Navigation

Links allow users to move from one webpage to another, jump to different sections of the same page, send emails, or download files. The navigation element helps organize these links into a menu.

---

## `<a>` (Anchor Tag)

### Description

The `<a>` tag is used to create a hyperlink. It allows users to navigate to another webpage, a specific section of the current page, an email address, or a downloadable file.

### Why We Use It

- Connect one webpage to another.
- Navigate to different sections of a page.
- Open external websites.
- Create email links.
- Allow file downloads.

### Syntax

```html
<a href="URL">Link Text</a>
```

### Example 1: Link to Another Website

```html
<a href="https://www.google.com">Visit Google</a>
```

### Explanation

Clicking **Visit Google** opens Google's website.

---

### Example 2: Open a Link in a New Tab

```html
<a href="https://www.github.com" target="_blank">Visit GitHub</a>
```

### Explanation

The `target="_blank"` attribute opens the webpage in a **new browser tab**.

---

### Example 3: Link to Another Section of the Same Page

```html
<a href="#contact">Go to Contact Section</a>
```

### Explanation

Clicking the link jumps to the element whose `id` is **contact**.

Example:

```html
<h2 id="contact">Contact Us</h2>
```

---

### Example 4: Email Link

```html
<a href="mailto:example@gmail.com">Send Email</a>
```

### Explanation

Clicking the link opens the user's default email application.

---

### Example 5: Telephone Link

```html
<a href="tel:+8801234567890">Call Us</a>
```

### Explanation

On mobile devices, clicking the link starts a phone call.

---

## Common Attributes of `<a>`

| Attribute | Description |
|-----------|-------------|
| `href` | Specifies the destination of the link. |
| `target` | Specifies where to open the linked page. |
| `title` | Displays a tooltip when hovering over the link. |
| `download` | Downloads the linked file instead of opening it. |

---

## `<nav>` (Navigation)

### Description

The `<nav>` tag represents a section of navigation links. It is commonly used to create menus for websites.

### Why We Use It

- Create navigation menus.
- Organize important links.
- Improve accessibility.
- Help search engines understand site navigation.

### Syntax

```html
<nav>Navigation Links</nav>
```

### Example

```html
<nav>
    <a href="#home">Home</a> |
    <a href="#about">About</a> |
    <a href="#services">Services</a> |
    <a href="#contact">Contact</a>
</nav>
```

### Explanation

This creates a simple navigation menu with four links.

---

## Complete Example

```html
<nav>
    <a href="#home">Home</a> |
    <a href="#about">About</a> |
    <a href="#contact">Contact</a>
</nav>

<hr>

<h2 id="home">Home</h2>
<p>Welcome to our website.</p>

<h2 id="about">About</h2>
<p>We provide web development tutorials.</p>

<h2 id="contact">Contact</h2>
<p>Email: example@gmail.com</p>
```

### Output

Home | About | Contact

---

Home

Welcome to our website.

---

About

We provide web development tutorials.

---

Contact

Email: example@gmail.com

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<a>` | Creates hyperlinks to webpages, sections, email addresses, phone numbers, or files. |
| `<nav>` | Groups navigation links together to create menus. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 7. Images & Media

HTML provides several elements for displaying images, playing audio and video, embedding other webpages, and creating graphics. These elements help make webpages more interactive and visually appealing.

---

## `<img>` (Image)

### Description

The `<img>` tag is used to display an image on a webpage.

### Why We Use It

- Display photos.
- Display logos.
- Display icons.
- Improve the appearance of a webpage.

### Syntax

```html
<img src="image.jpg" alt="Description">
```

### Example

```html
<img src="logo.png" alt="Company Logo" width="200">
```

### Explanation

This displays an image named **logo.png** with a width of **200 pixels**. The `alt` attribute provides alternative text if the image cannot be displayed.

---

## `<figure>`

### Description

The `<figure>` tag groups an image, diagram, or other media together with its caption.

### Why We Use It

- Organize images with captions.
- Improve webpage structure.
- Make content easier to understand.

### Syntax

```html
<figure>...</figure>
```

### Example

```html
<figure>
    <img src="flower.jpg" alt="Flower">
    <figcaption>A beautiful flower.</figcaption>
</figure>
```

### Explanation

The image and its caption are grouped together as one unit.

---

## `<figcaption>`

### Description

The `<figcaption>` tag provides a caption for the content inside a `<figure>` element.

### Why We Use It

- Add descriptions to images.
- Label diagrams or charts.
- Improve accessibility.

### Syntax

```html
<figcaption>Caption</figcaption>
```

### Example

```html
<figcaption>Figure 1: Company Logo</figcaption>
```

### Explanation

Displays a caption below or above the image inside the `<figure>` element.

---

## `<picture>`

### Description

The `<picture>` tag allows you to provide multiple versions of an image. The browser automatically selects the most suitable one.

### Why We Use It

- Create responsive images.
- Display different images for different screen sizes.

### Syntax

```html
<picture>...</picture>
```

### Example

```html
<picture>
    <source media="(min-width:600px)" srcset="large.jpg">
    <img src="small.jpg" alt="Responsive Image">
</picture>
```

### Explanation

Large screens display **large.jpg**, while smaller screens display **small.jpg**.

---

## `<source>`

### Description

The `<source>` tag specifies different media files for `<picture>`, `<audio>`, or `<video>`.

### Why We Use It

- Provide multiple file formats.
- Improve browser compatibility.

### Syntax

```html
<source src="file.mp4" type="video/mp4">
```

### Example

```html
<source src="song.mp3" type="audio/mpeg">
```

### Explanation

The browser loads the specified media file if it supports the format.

---

## `<audio>`

### Description

The `<audio>` tag is used to play audio files on a webpage.

### Why We Use It

- Play music.
- Add podcasts.
- Play sound effects.

### Syntax

```html
<audio controls></audio>
```

### Example

```html
<audio controls>
    <source src="song.mp3" type="audio/mpeg">
</audio>
```

### Explanation

A built-in audio player appears with play, pause, and volume controls.

---

## `<video>`

### Description

The `<video>` tag is used to play videos on a webpage.

### Why We Use It

- Display tutorials.
- Play movies.
- Embed educational videos.

### Syntax

```html
<video controls></video>
```

### Example

```html
<video controls width="400">
    <source src="video.mp4" type="video/mp4">
</video>
```

### Explanation

A video player appears with playback controls.

---

## `<track>`

### Description

The `<track>` tag adds subtitles or captions to a video.

### Why We Use It

- Display subtitles.
- Improve accessibility.
- Support multiple languages.

### Syntax

```html
<track src="subtitle.vtt">
```

### Example

```html
<track src="english.vtt" kind="subtitles" srclang="en" label="English">
```

### Explanation

Displays English subtitles while the video is playing.

---

## `<iframe>`

### Description

The `<iframe>` tag embeds another webpage inside the current webpage.

### Why We Use It

- Embed YouTube videos.
- Display Google Maps.
- Embed another website.

### Syntax

```html
<iframe src="URL"></iframe>
```

### Example

```html
<iframe src="https://example.com" width="400" height="250"></iframe>
```

### Explanation

The webpage from **example.com** appears inside the current webpage.

---

## `<embed>`

### Description

The `<embed>` tag embeds external files such as PDFs or multimedia content.

### Why We Use It

- Display PDF files.
- Embed multimedia.
- Show external documents.

### Syntax

```html
<embed src="file.pdf">
```

### Example

```html
<embed src="notes.pdf" width="400" height="300">
```

### Explanation

The PDF file is displayed inside the webpage.

---

## `<object>`

### Description

The `<object>` tag embeds external resources such as PDFs, images, or multimedia.

### Why We Use It

- Display documents.
- Embed external content.
- Provide alternative content if needed.

### Syntax

```html
<object data="file.pdf"></object>
```

### Example

```html
<object data="notes.pdf" width="400" height="300"></object>
```

### Explanation

Displays the PDF file within the webpage.

---

## `<canvas>`

### Description

The `<canvas>` tag provides a blank area where graphics can be drawn using JavaScript.

### Why We Use It

- Draw shapes.
- Create games.
- Display charts.
- Create animations.

### Syntax

```html
<canvas></canvas>
```

### Example

```html
<canvas id="myCanvas" width="300" height="150"></canvas>
```

### Explanation

Creates an empty drawing area that JavaScript can use.

---

## `<svg>`

### Description

The `<svg>` tag is used to create scalable vector graphics directly in HTML.

### Why We Use It

- Draw shapes.
- Create logos.
- Display icons.
- Create diagrams.

### Syntax

```html
<svg></svg>
```

### Example

```html
<svg width="100" height="100">
    <circle cx="50" cy="50" r="40" fill="blue"/>
</svg>
```

### Explanation

Displays a blue circle using vector graphics.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<img>` | Displays an image. |
| `<figure>` | Groups media with a caption. |
| `<figcaption>` | Adds a caption to a figure. |
| `<picture>` | Displays responsive images. |
| `<source>` | Specifies media sources. |
| `<audio>` | Plays audio files. |
| `<video>` | Plays video files. |
| `<track>` | Adds subtitles or captions to videos. |
| `<iframe>` | Embeds another webpage. |
| `<embed>` | Embeds external files such as PDFs. |
| `<object>` | Embeds external resources. |
| `<canvas>` | Creates a drawing area for JavaScript graphics. |
| `<svg>` | Creates scalable vector graphics. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 8. Tables

Tables are used to organize data into **rows and columns**. They are useful for displaying structured information such as student marks, employee records, product lists, schedules, and more.

---

## `<table>`

### Description

The `<table>` tag creates a table.

### Why We Use It

- Display data in rows and columns.
- Organize structured information.
- Improve readability.

### Syntax

```html
<table>
    ...
</table>
```

### Example

```html
<table></table>
```

### Explanation

This creates the main container for a table.

---

## `<caption>`

### Description

The `<caption>` tag adds a title to a table.

### Why We Use It

- Give the table a title.
- Explain what the table is about.
- Improve accessibility.

### Syntax

```html
<caption>Table Title</caption>
```

### Example

```html
<caption>Student Marks</caption>
```

### Explanation

The title appears above the table.

---

## `<colgroup>`

### Description

The `<colgroup>` tag groups one or more columns together for formatting.

### Why We Use It

- Apply styles to multiple columns.
- Organize table columns.

### Syntax

```html
<colgroup>
    <col>
</colgroup>
```

### Example

```html
<colgroup>
    <col style="background-color: lightgray;">
</colgroup>
```

### Explanation

The first column will have a light gray background.

---

## `<col>`

### Description

The `<col>` tag defines properties for one or more columns inside a `<colgroup>`.

### Why We Use It

- Style entire columns.
- Set column width.
- Change column colors.

### Syntax

```html
<col>
```

### Example

```html
<col style="width:150px;">
```

### Explanation

The selected column will have a width of **150 pixels**.

---

## `<thead>`

### Description

The `<thead>` tag groups the header rows of a table.

### Why We Use It

- Separate the table header.
- Improve readability.
- Make table styling easier.

### Syntax

```html
<thead>
    ...
</thead>
```

### Example

```html
<thead>
    <tr>
        <th>Name</th>
        <th>Marks</th>
    </tr>
</thead>
```

### Explanation

This defines the header section of the table.

---

## `<tbody>`

### Description

The `<tbody>` tag groups the main data rows of a table.

### Why We Use It

- Separate table data from the header and footer.
- Organize large tables.

### Syntax

```html
<tbody>
    ...
</tbody>
```

### Example

```html
<tbody>
    <tr>
        <td>John</td>
        <td>90</td>
    </tr>
</tbody>
```

### Explanation

This contains the main content of the table.

---

## `<tfoot>`

### Description

The `<tfoot>` tag groups the footer rows of a table.

### Why We Use It

- Display totals.
- Show summaries.
- Add notes at the bottom of a table.

### Syntax

```html
<tfoot>
    ...
</tfoot>
```

### Example

```html
<tfoot>
    <tr>
        <td>Total</td>
        <td>90</td>
    </tr>
</tfoot>
```

### Explanation

This creates the footer section of the table.

---

## `<tr>` (Table Row)

### Description

The `<tr>` tag creates a row inside a table.

### Why We Use It

- Add new rows.
- Organize table data.

### Syntax

```html
<tr>
    ...
</tr>
```

### Example

```html
<tr>
    <td>John</td>
    <td>90</td>
</tr>
```

### Explanation

This creates one row containing two cells.

---

## `<th>` (Table Header)

### Description

The `<th>` tag creates a header cell in a table.

### Why We Use It

- Display column names.
- Make headings bold by default.
- Improve accessibility.

### Syntax

```html
<th>Heading</th>
```

### Example

```html
<th>Name</th>
```

### Explanation

This creates a header cell with the text **Name**.

---

## `<td>` (Table Data)

### Description

The `<td>` tag creates a normal data cell inside a table.

### Why We Use It

- Store table data.
- Display information in rows and columns.

### Syntax

```html
<td>Data</td>
```

### Example

```html
<td>90</td>
```

### Explanation

This creates a table cell containing the value **90**.

---

## Complete Example

```html
<table border="1">

    <caption>Student Marks</caption>

    <colgroup>
        <col style="background-color: lightyellow;">
        <col>
    </colgroup>

    <thead>
        <tr>
            <th>Name</th>
            <th>Marks</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>John</td>
            <td>90</td>
        </tr>

        <tr>
            <td>Emma</td>
            <td>95</td>
        </tr>
    </tbody>

    <tfoot>
        <tr>
            <td>Average</td>
            <td>92.5</td>
        </tr>
    </tfoot>

</table>
```

### Output

| Name | Marks |
|------|------:|
| John | 90 |
| Emma | 95 |
| **Average** | **92.5** |

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<table>` | Creates a table. |
| `<caption>` | Adds a title to the table. |
| `<colgroup>` | Groups table columns for formatting. |
| `<col>` | Defines properties of a column. |
| `<thead>` | Groups the table header. |
| `<tbody>` | Groups the main table data. |
| `<tfoot>` | Groups the table footer. |
| `<tr>` | Creates a table row. |
| `<th>` | Creates a table header cell. |
| `<td>` | Creates a table data cell. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 9. Forms & Input

Forms are used to collect information from users. They allow users to enter text, choose options, upload files, submit data, and interact with a webpage.

---

## `<form>`

### Description

The `<form>` tag creates an HTML form that collects user input.

### Why We Use It

- Collect user information.
- Create login and registration forms.
- Submit data to a server.

### Syntax

```html
<form action="URL" method="GET or POST">
    Form Elements
</form>
```

### Example

```html
<form action="/submit" method="post"></form>
```

### Explanation

The form sends user data to **/submit** using the **POST** method.

---

## Common Attributes of `<form>`

| Attribute | Description |
|-----------|-------------|
| `action` | Specifies where the form data is sent. |
| `method` | Specifies how data is sent (`GET` or `POST`). |
| `autocomplete` | Turns autocomplete on or off. |
| `target` | Specifies where to display the response. |

---

## `<input>`

### Description

The `<input>` tag creates different types of input fields.

### Why We Use It

- Enter text.
- Enter passwords.
- Select dates.
- Upload files.
- Choose options.

### Syntax

```html
<input type="text">
```

### Example

```html
<input type="text" placeholder="Enter your name">
```

### Explanation

Creates a text box where the user can enter their name.

---

## Common Input Types

| Type | Purpose |
|------|---------|
| `text` | Single-line text input |
| `password` | Password field |
| `email` | Email address |
| `number` | Numeric input |
| `date` | Date picker |
| `time` | Time picker |
| `checkbox` | Select multiple options |
| `radio` | Select one option |
| `file` | Upload a file |
| `submit` | Submit the form |
| `reset` | Reset all fields |
| `button` | Create a button |
| `color` | Color picker |
| `range` | Slider |
| `url` | Website URL |
| `tel` | Phone number |

---

## Common Attributes of `<input>`

| Attribute | Description |
|-----------|-------------|
| `type` | Specifies the type of input field. |
| `name` | Identifies the input when submitting the form. |
| `id` | Gives the input a unique identifier. |
| `placeholder` | Displays a hint inside the input box. |
| `value` | Sets the default value. |
| `required` | Makes the field mandatory. |
| `readonly` | Prevents editing. |
| `disabled` | Disables the input field. |
| `maxlength` | Sets the maximum number of characters. |

---

## `<label>`

### Description

The `<label>` tag provides a label for an input field.

### Why We Use It

- Improve accessibility.
- Make forms easier to understand.

### Syntax

```html
<label for="id">Label</label>
```

### Example

```html
<label for="name">Name:</label>
```

### Explanation

Displays **Name:** as the label for the input field.

---

## `<textarea>`

### Description

The `<textarea>` tag creates a multi-line text input area.

### Why We Use It

- Collect comments.
- Collect feedback.
- Write messages.

### Syntax

```html
<textarea></textarea>
```

### Example

```html
<textarea rows="4" cols="30"></textarea>
```

### Explanation

Creates a text area with 4 rows and 30 columns.

---

## `<button>`

### Description

The `<button>` tag creates a clickable button.

### Why We Use It

- Submit forms.
- Reset forms.
- Perform JavaScript actions.

### Syntax

```html
<button>Button</button>
```

### Example

```html
<button type="submit">Submit</button>
```

### Explanation

Creates a button that submits the form.

---

## `<select>`

### Description

The `<select>` tag creates a drop-down list.

### Why We Use It

- Let users choose one option.
- Save space on forms.

### Syntax

```html
<select></select>
```

### Example

```html
<select>
    <option>HTML</option>
    <option>CSS</option>
</select>
```

### Explanation

Creates a drop-down menu with two options.

---

## `<option>`

### Description

The `<option>` tag defines an item inside a drop-down list.

### Why We Use It

- Add choices to a `<select>` element.

### Syntax

```html
<option>Option</option>
```

### Example

```html
<option>JavaScript</option>
```

### Explanation

Adds **JavaScript** as one option in the drop-down list.

---

## `<optgroup>`

### Description

The `<optgroup>` tag groups related options inside a drop-down list.

### Why We Use It

- Organize large lists.
- Improve readability.

### Syntax

```html
<optgroup label="Group"></optgroup>
```

### Example

```html
<optgroup label="Programming">
    <option>HTML</option>
    <option>CSS</option>
</optgroup>
```

### Explanation

Groups HTML and CSS under the heading **Programming**.

---

## `<fieldset>`

### Description

The `<fieldset>` tag groups related form elements together.

### Why We Use It

- Organize forms.
- Improve readability.

### Syntax

```html
<fieldset></fieldset>
```

### Example

```html
<fieldset>
    <legend>Personal Information</legend>
</fieldset>
```

### Explanation

Creates a bordered section for related form fields.

---

## `<legend>`

### Description

The `<legend>` tag adds a title to a `<fieldset>`.

### Why We Use It

- Describe grouped form fields.
- Improve form organization.

### Syntax

```html
<legend>Title</legend>
```

### Example

```html
<legend>Login Form</legend>
```

### Explanation

Displays **Login Form** as the title of the fieldset.

---

## `<datalist>`

### Description

The `<datalist>` tag provides predefined suggestions for an input field.

### Why We Use It

- Show autocomplete suggestions.
- Help users enter values quickly.

### Syntax

```html
<datalist></datalist>
```

### Example

```html
<input list="browsers">

<datalist id="browsers">
    <option value="Chrome">
    <option value="Firefox">
</datalist>
```

### Explanation

The user receives suggestions while typing.

---

## `<output>`

### Description

The `<output>` tag displays the result of a calculation or user action.

### Why We Use It

- Show calculated values.
- Display dynamic results.

### Syntax

```html
<output></output>
```

### Example

```html
<output>100</output>
```

### Explanation

Displays the value **100** as the output.

---

## Complete Example

```html
<form action="/submit" method="post">

    <fieldset>

        <legend>Student Registration</legend>

        <label>Name:</label><br>
        <input type="text" placeholder="Enter your name" required><br><br>

        <label>Email:</label><br>
        <input type="email" placeholder="Enter your email"><br><br>

        <label>Course:</label><br>

        <select>
            <option>HTML</option>
            <option>CSS</option>
            <option>JavaScript</option>
        </select>

        <br><br>

        <label>Comments:</label><br>
        <textarea rows="4" cols="30"></textarea>

        <br><br>

        <button type="submit">Submit</button>

    </fieldset>

</form>
```

### Output

- A registration form with:
  - Name input box
  - Email input box
  - Course drop-down list
  - Comments text area
  - Submit button

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<form>` | Creates a form. |
| `<input>` | Creates different types of input fields. |
| `<label>` | Adds a label to an input field. |
| `<textarea>` | Creates a multi-line text box. |
| `<button>` | Creates a clickable button. |
| `<select>` | Creates a drop-down list. |
| `<option>` | Adds an option to a drop-down list. |
| `<optgroup>` | Groups related options. |
| `<fieldset>` | Groups related form elements. |
| `<legend>` | Adds a title to a fieldset. |
| `<datalist>` | Provides input suggestions. |
| `<output>` | Displays the result of a calculation or action. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 10. Semantic Layout (HTML5)

Semantic HTML5 elements describe the **meaning and purpose** of different parts of a webpage. They make webpages easier to read, improve accessibility, and help search engines understand the page structure.

---

## `<header>`

### Description

The `<header>` tag represents the introductory section of a webpage or a section.

### Why We Use It

- Display the website logo.
- Display the page title.
- Display the navigation menu.

### Syntax

```html
<header>
    Content
</header>
```

### Example

```html
<header>
    <h1>HTML Reference Guide</h1>
</header>
```

### Explanation

This creates the top section of the webpage containing the main heading.

---

## `<nav>`

### Description

The `<nav>` tag defines a section that contains navigation links.

### Why We Use It

- Create navigation menus.
- Organize important links.
- Improve accessibility.

### Syntax

```html
<nav>
    Links
</nav>
```

### Example

```html
<nav>
    <a href="#">Home</a>
    <a href="#">About</a>
</nav>
```

### Explanation

This creates a simple navigation menu with links.

---

## `<main>`

### Description

The `<main>` tag contains the primary content of the webpage.

### Why We Use It

- Hold the main content.
- Improve webpage structure.
- Help screen readers identify the important content.

### Syntax

```html
<main>
    Content
</main>
```

### Example

```html
<main>
    <h2>Welcome</h2>
    <p>This is the main content.</p>
</main>
```

### Explanation

Everything inside `<main>` represents the central content of the webpage.

---

## `<section>`

### Description

The `<section>` tag groups related content into a section.

### Why We Use It

- Divide content into sections.
- Organize webpages.
- Improve readability.

### Syntax

```html
<section>
    Content
</section>
```

### Example

```html
<section>
    <h2>Our Services</h2>
</section>
```

### Explanation

This creates a separate section for the services.

---

## `<article>`

### Description

The `<article>` tag represents independent content that can stand alone.

### Why We Use It

- Blog posts.
- News articles.
- Forum posts.
- Product reviews.

### Syntax

```html
<article>
    Content
</article>
```

### Example

```html
<article>
    <h2>Learning HTML</h2>
    <p>HTML is easy to learn.</p>
</article>
```

### Explanation

This creates a self-contained article.

---

## `<aside>`

### Description

The `<aside>` tag contains content that is related to the main content but not part of it.

### Why We Use It

- Display advertisements.
- Show related links.
- Add sidebars.
- Display additional information.

### Syntax

```html
<aside>
    Content
</aside>
```

### Example

```html
<aside>
    Related Articles
</aside>
```

### Explanation

This creates a sidebar containing related content.

---

## `<footer>`

### Description

The `<footer>` tag represents the bottom section of a webpage or section.

### Why We Use It

- Display copyright information.
- Display contact details.
- Display social media links.
- Display useful links.

### Syntax

```html
<footer>
    Content
</footer>
```

### Example

```html
<footer>
    © 2026 HTML Reference Guide
</footer>
```

### Explanation

This creates the footer at the bottom of the webpage.

---

## Complete Example

```html
<header>
    <h1>HTML Reference Guide</h1>
</header>

<nav>
    <a href="#">Home</a> |
    <a href="#">About</a> |
    <a href="#">Contact</a>
</nav>

<main>

    <section>
        <h2>Our Courses</h2>
        <p>Learn HTML from beginner to advanced.</p>
    </section>

    <article>
        <h2>Latest Article</h2>
        <p>Semantic HTML improves webpage structure.</p>
    </article>

    <aside>
        <h3>Related Topics</h3>
        <p>CSS, JavaScript, Bootstrap</p>
    </aside>

</main>

<footer>
    © 2026 HTML Reference Guide
</footer>
```

### Output

- **Header** containing the website title.
- **Navigation menu** with links.
- **Main content** section.
- **Article** displaying independent content.
- **Sidebar** showing related topics.
- **Footer** containing copyright information.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<header>` | Defines the top section of a webpage or section. |
| `<nav>` | Contains navigation links. |
| `<main>` | Holds the main content of the webpage. |
| `<section>` | Groups related content together. |
| `<article>` | Represents independent, self-contained content. |
| `<aside>` | Contains related or sidebar content. |
| `<footer>` | Defines the bottom section of a webpage or section. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 11. Scripting & Templates

Scripting and template elements are used to add interactivity, include external JavaScript files, provide fallback content when JavaScript is disabled, and create reusable HTML templates.

---

## `<script>`

### Description

The `<script>` tag is used to add JavaScript code to a webpage or link an external JavaScript file.

### Why We Use It

- Make webpages interactive.
- Validate forms.
- Handle user events.
- Create animations.
- Connect external JavaScript files.

### Syntax

```html
<script>
    JavaScript Code
</script>
```

### Example 1: Internal JavaScript

```html
<script>
    alert("Welcome to HTML!");
</script>
```

### Explanation

When the webpage loads, a popup message saying **"Welcome to HTML!"** appears.

---

### Example 2: External JavaScript

```html
<script src="script.js"></script>
```

### Explanation

This loads and runs the JavaScript code stored in the **script.js** file.

---

## Common Attributes of `<script>`

| Attribute | Description |
|-----------|-------------|
| `src` | Specifies an external JavaScript file. |
| `type` | Specifies the scripting language (optional in HTML5). |
| `defer` | Loads the script after the HTML document has been parsed. |
| `async` | Loads the script asynchronously without blocking the page. |

---

## `<noscript>`

### Description

The `<noscript>` tag displays content only when JavaScript is disabled or not supported by the browser.

### Why We Use It

- Inform users that JavaScript is required.
- Provide alternative content.
- Improve user experience.

### Syntax

```html
<noscript>
    Message
</noscript>
```

### Example

```html
<noscript>
    Please enable JavaScript to use this website.
</noscript>
```

### Explanation

If JavaScript is disabled, this message is displayed to the user.

---

## `<template>`

### Description

The `<template>` tag stores HTML content that is **not displayed immediately**. It can be used later with JavaScript.

### Why We Use It

- Create reusable HTML content.
- Build dynamic webpages.
- Avoid repeating HTML code.

### Syntax

```html
<template>
    HTML Content
</template>
```

### Example

```html
<template id="card">
    <h2>HTML Tutorial</h2>
    <p>Welcome to HTML Reference Guide.</p>
</template>
```

### Explanation

The content inside the template is stored but is **not shown** until JavaScript uses it.

---

## `<slot>`

### Description

The `<slot>` tag is used inside Web Components to define where custom content should appear.

### Why We Use It

- Create reusable custom components.
- Insert user-provided content into templates.
- Build modern web applications.

### Syntax

```html
<slot></slot>
```

### Example

```html
<slot></slot>
```

### Explanation

When using Web Components, the `<slot>` element acts as a placeholder where content is inserted.

> **Note:** Beginners usually don't use `<slot>`. It is mainly used in advanced HTML with Web Components.

---

## Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>Scripting Example</title>
</head>

<body>

    <h1>HTML Reference Guide</h1>

    <script>
        alert("Welcome!");
    </script>

    <noscript>
        Please enable JavaScript to view this website properly.
    </noscript>

    <template id="message">
        <h2>Hello, Student!</h2>
        <p>Keep learning HTML.</p>
    </template>

</body>

</html>
```

### Output

- The webpage displays the heading **HTML Reference Guide**.
- A popup appears saying **"Welcome!"**.
- If JavaScript is disabled, the message **"Please enable JavaScript to view this website properly."** is shown.
- The template content remains hidden until JavaScript displays it.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<script>` | Adds or links JavaScript code. |
| `<noscript>` | Displays content when JavaScript is disabled. |
| `<template>` | Stores reusable HTML content that is hidden until needed. |
| `<slot>` | Defines a placeholder for content inside Web Components. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 12. Interactive & Miscellaneous

Interactive HTML elements allow users to interact with a webpage without using much JavaScript. These elements can create expandable sections, dialogs, progress indicators, measurements, and other useful interface components.

---

## `<details>`

### Description

The `<details>` tag creates a section that users can expand or collapse.

### Why We Use It

- Hide extra information.
- Create FAQs.
- Save space on a webpage.

### Syntax

```html
<details>
    Content
</details>
```

### Example

```html
<details>
    <summary>Click to Learn More</summary>
    HTML is the standard markup language for creating web pages.
</details>
```

### Explanation

Clicking **"Click to Learn More"** expands or collapses the hidden content.

---

## `<summary>`

### Description

The `<summary>` tag defines the visible heading for a `<details>` element.

### Why We Use It

- Create clickable headings.
- Show or hide content.

### Syntax

```html
<summary>Title</summary>
```

### Example

```html
<summary>Frequently Asked Questions</summary>
```

### Explanation

The text becomes the clickable title of the expandable section.

---

## `<dialog>`

### Description

The `<dialog>` tag creates a dialog box or popup window.

### Why We Use It

- Display notifications.
- Show confirmation messages.
- Create popup windows.

### Syntax

```html
<dialog>
    Content
</dialog>
```

### Example

```html
<dialog open>
    Welcome to HTML Reference Guide!
</dialog>
```

### Explanation

The dialog box appears immediately because of the **open** attribute.

---

## `<progress>`

### Description

The `<progress>` tag displays the progress of a task.

### Why We Use It

- Show download progress.
- Display upload status.
- Track task completion.

### Syntax

```html
<progress value="50" max="100"></progress>
```

### Example

```html
<progress value="70" max="100"></progress>
```

### Explanation

The progress bar shows that **70%** of the task is completed.

---

## `<meter>`

### Description

The `<meter>` tag displays a value within a known range.

### Why We Use It

- Show battery level.
- Display disk usage.
- Display scores or ratings.

### Syntax

```html
<meter value="0.6"></meter>
```

### Example

```html
<meter value="80" min="0" max="100"></meter>
```

### Explanation

The meter indicates a value of **80 out of 100**.

---

## `<data>`

### Description

The `<data>` tag associates visible content with a machine-readable value.

### Why We Use It

- Store product IDs.
- Store numerical values.
- Help computers understand displayed data.

### Syntax

```html
<data value="123">Product</data>
```

### Example

```html
<data value="101">Laptop</data>
```

### Explanation

The user sees **Laptop**, while the machine-readable value is **101**.

---

## `<bdi>`

### Description

The `<bdi>` tag isolates text that may have a different writing direction from the surrounding text.

### Why We Use It

- Display multilingual text.
- Prevent text direction problems.

### Syntax

```html
<bdi>Text</bdi>
```

### Example

```html
<bdi>مرحبا</bdi>
```

### Explanation

The browser displays the text with its correct writing direction.

---

## `<bdo>`

### Description

The `<bdo>` tag overrides the default text direction.

### Why We Use It

- Display text from right to left.
- Display text from left to right.

### Syntax

```html
<bdo dir="rtl">Text</bdo>
```

### Example

```html
<bdo dir="rtl">HTML</bdo>
```

### Explanation

The text is displayed from **right to left**.

---

## `<ruby>`

### Description

The `<ruby>` tag displays pronunciation or annotations above or beside characters.

### Why We Use It

- Display pronunciation guides.
- Help readers understand foreign languages.

### Syntax

```html
<ruby>Text</ruby>
```

### Example

```html
<ruby>
    漢
    <rt>Kan</rt>
</ruby>
```

### Explanation

The pronunciation **Kan** appears above or beside the character.

---

## `<rt>`

### Description

The `<rt>` tag defines the pronunciation or explanation inside a `<ruby>` element.

### Why We Use It

- Display pronunciation.
- Add reading guides.

### Syntax

```html
<rt>Pronunciation</rt>
```

### Example

```html
<rt>Kan</rt>
```

### Explanation

Displays the pronunciation for the associated character.

---

## `<rp>`

### Description

The `<rp>` tag provides fallback parentheses for browsers that do not support ruby annotations.

### Why We Use It

- Improve compatibility.
- Provide fallback text.

### Syntax

```html
<rp>(</rp>
```

### Example

```html
<rp>(</rp>
<rt>Kan</rt>
<rp>)</rp>
```

### Explanation

Older browsers display the pronunciation inside parentheses.

---

## Complete Example

```html
<details>
    <summary>HTML Tutorial</summary>
    HTML is easy to learn.
</details>

<br>

<dialog open>
    Welcome to HTML Reference Guide!
</dialog>

<br><br>

<label>Course Progress:</label>

<progress value="75" max="100"></progress>

<br><br>

<label>Battery Level:</label>

<meter value="90" min="0" max="100"></meter>
```

### Output

- An expandable **HTML Tutorial** section.
- A popup dialog saying **Welcome to HTML Reference Guide!**
- A progress bar showing **75% completion**.
- A meter displaying **90% battery level**.

---

## 📌 Summary

| Element | Purpose |
|---------|---------|
| `<details>` | Creates expandable and collapsible content. |
| `<summary>` | Defines the heading for a `<details>` element. |
| `<dialog>` | Creates a dialog box or popup. |
| `<progress>` | Displays the progress of a task. |
| `<meter>` | Displays a value within a known range. |
| `<data>` | Associates visible content with a machine-readable value. |
| `<bdi>` | Isolates text with a different writing direction. |
| `<bdo>` | Overrides the text direction. |
| `<ruby>` | Displays pronunciation or annotations. |
| `<rt>` | Defines the pronunciation inside a `<ruby>` element. |
| `<rp>` | Provides fallback text for ruby annotations. |

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)

---
---

# 13. Deprecated Tags (Good to Recognize, Avoid Using)

Deprecated HTML tags are elements that were used in older versions of HTML but are **no longer recommended in HTML5**. Modern HTML uses **CSS** and newer semantic elements instead.

> **Note:** You may still see these tags in old websites, but you should avoid using them in new projects.

---

## `<font>`

### Description

The `<font>` tag was used to change the font size, color, and font family.

### Why It Was Used

- Change text color.
- Change font size.
- Change font style.

### Syntax

```html
<font color="red">Text</font>
```

### Example

```html
<font color="blue">Hello World</font>
```

### Explanation

The text appears in blue.

### Modern Alternative

Use **CSS** instead.

```html
<p style="color: blue;">Hello World</p>
```

---

## `<center>`

### Description

The `<center>` tag was used to center content on a webpage.

### Why It Was Used

- Center text.
- Center images.
- Center tables.

### Syntax

```html
<center>Content</center>
```

### Example

```html
<center>Welcome to HTML</center>
```

### Explanation

The text appears in the center of the page.

### Modern Alternative

Use CSS.

```html
<p style="text-align: center;">Welcome to HTML</p>
```

---

## `<marquee>`

### Description

The `<marquee>` tag creates scrolling text or images.

### Why It Was Used

- Display moving announcements.
- Create scrolling news.

### Syntax

```html
<marquee>Text</marquee>
```

### Example

```html
<marquee>Welcome to HTML Reference Guide!</marquee>
```

### Explanation

The text scrolls across the screen.

### Modern Alternative

Use **CSS Animations**.

---

## `<big>`

### Description

The `<big>` tag displays text one size larger than normal.

### Why It Was Used

- Increase text size.

### Syntax

```html
<big>Text</big>
```

### Example

```html
<big>Hello</big>
```

### Explanation

The word **Hello** appears larger.

### Modern Alternative

Use CSS.

```html
<p style="font-size: 24px;">Hello</p>
```

---

## `<tt>`

### Description

The `<tt>` tag displayed text in a monospace (typewriter) font.

### Why It Was Used

- Display computer code.
- Display commands.

### Syntax

```html
<tt>Text</tt>
```

### Example

```html
<tt>console.log()</tt>
```

### Explanation

The text appears in a typewriter-style font.

### Modern Alternative

Use the `<code>` element.

```html
<code>console.log()</code>
```

---

## `<strike>`

### Description

The `<strike>` tag displayed text with a line through it.

### Why It Was Used

- Show removed text.
- Display old prices.

### Syntax

```html
<strike>Text</strike>
```

### Example

```html
<strike>$100</strike>
```

### Explanation

The old price appears with a line through it.

### Modern Alternative

Use the `<del>` element.

```html
<del>$100</del>
```

---

## `<acronym>`

### Description

The `<acronym>` tag defined an acronym.

### Why It Was Used

- Explain abbreviations.

### Syntax

```html
<acronym title="Meaning">ABC</acronym>
```

### Example

```html
<acronym title="HyperText Markup Language">HTML</acronym>
```

### Explanation

Shows the full meaning when the user hovers over the text.

### Modern Alternative

Use the `<abbr>` element.

```html
<abbr title="HyperText Markup Language">HTML</abbr>
```

---

## `<dir>`

### Description

The `<dir>` tag was used to create a directory list.

### Why It Was Used

- Display lists.

### Syntax

```html
<dir>
    <li>Item</li>
</dir>
```

### Example

```html
<dir>
    <li>HTML</li>
</dir>
```

### Explanation

Displays a directory-style list.

### Modern Alternative

Use `<ul>`.

```html
<ul>
    <li>HTML</li>
</ul>
```

---

## `<frame>`

### Description

The `<frame>` tag displayed another HTML document inside a frame.

### Why It Was Used

- Divide the browser window into multiple sections.

### Syntax

```html
<frame src="page.html">
```

### Example

```html
<frame src="home.html">
```

### Explanation

Displays another webpage inside a frame.

### Modern Alternative

Use `<iframe>`.

```html
<iframe src="home.html"></iframe>
```

---

## `<frameset>`

### Description

The `<frameset>` tag defined multiple frames in one browser window.

### Why It Was Used

- Split the browser window into frames.

### Syntax

```html
<frameset cols="50%,50%">
</frameset>
```

### Example

```html
<frameset cols="30%,70%">
</frameset>
```

### Explanation

Divides the browser window into two sections.

### Modern Alternative

Use CSS layouts with `<div>`, `<section>`, or `<iframe>`.

---

## 📌 Summary

| Deprecated Tag | Modern Alternative |
|----------------|--------------------|
| `<font>` | CSS (`color`, `font-size`, `font-family`) |
| `<center>` | CSS (`text-align: center`) |
| `<marquee>` | CSS Animations |
| `<big>` | CSS (`font-size`) |
| `<tt>` | `<code>` |
| `<strike>` | `<del>` |
| `<acronym>` | `<abbr>` |
| `<dir>` | `<ul>` |
| `<frame>` | `<iframe>` |
| `<frameset>` | CSS Layout + `<iframe>` |

---

## 🎉 Congratulations!

You have completed this **HTML Reference Guide** guide!

By finishing these chapters, you have learned:

- ✅ Document Structure
- ✅ Metadata & Head Elements
- ✅ Headings & Text Content
- ✅ Text Formatting & Inline Semantics
- ✅ Lists
- ✅ Links & Navigation
- ✅ Images & Media
- ✅ Tables
- ✅ Forms & Input
- ✅ Semantic Layout (HTML5)
- ✅ Scripting & Templates
- ✅ Interactive & Miscellaneous
- ✅ Deprecated HTML Tags

Keep practicing by building your own webpages. The more you code, the more confident you'll become with HTML.

Happy Coding! 🚀

---

⬆️ **Back to:** [Table of Contents](#-table-of-contents)


