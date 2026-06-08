# 🚀 Frontend Essentials Bootcamp 2026

<div align="center">

## 📘 Module 1: HTML Foundation


</div>

---

# 📌 Introduction to Frontend Development

Frontend development is the process of building the **visible** and **interactive** portion of websites and web applications that users directly interact with inside a web browser.

Modern frontend engineering focuses on:

* ✅ Structured and semantic markup
* ✅ Responsive layouts
* ✅ Accessibility standards
* ✅ User experience (UX)
* ✅ Web performance optimization
* ✅ Browser compatibility

---

# 🛠️ Core Frontend Technologies

| Technology   | Purpose               |
| ------------ | --------------------- |
| 🌐 HTML      | Structure of Webpages |
| 🎨 CSS       | Styling & Layout      |
| ⚡ JavaScript | Interactivity & Logic |

---

# 🌐 Understanding How Websites Work

When a user opens a website, several processes occur behind the scenes.

## 🔄 Basic Web Flow

```txt
User → Browser → Server → HTML/CSS/JS → Browser Rendering
```

## 📖 Step-by-Step Process

1. 🌍 The browser sends a request to a web server.
2. 📦 The server returns HTML, CSS, JavaScript, images, and other resources.
3. 🧠 The browser parses and renders these files.
4. 🖥️ The webpage becomes visible and interactive.

---

# 🏗️ HTML Document Structure

Every HTML document follows a standard structure called the **HTML Boilerplate**.

## 📄 Standard HTML5 Boilerplate

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Frontend Essentials Bootcamp 2026</title>
</head>

<body>

</body>

</html>
```

---

# 🔍 Important HTML Elements Explained

## `<!DOCTYPE html>`

✅ Defines the document type and tells the browser to use HTML5 standards.

---

## `<html>`

✅ Root element that wraps the complete webpage.

```html
<html lang="en">
```

---

## `<head>`

✅ Contains metadata, SEO information, stylesheets, and page configuration.

```html
<head>
    <title>My Website</title>
</head>
```

---

## `<meta charset="UTF-8">`

✅ Supports global characters and symbols.

```html
<meta charset="UTF-8">
```

---

## `<meta name="viewport">`

✅ Makes webpages responsive on mobile devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

## `<title>`

✅ Defines the browser tab title and improves SEO.

```html
<title>Frontend Essentials Bootcamp</title>
```

---

## `<body>`

✅ Contains all visible webpage content.

```html
<body>
    <h1>Hello World</h1>
</body>
```

---

# 📝 Headings and Paragraphs

HTML provides heading tags from `<h1>` to `<h6>`.

## 📌 Example

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Section Heading</h3>
```

---

# ✅ Best Practices for Headings

* Use only **one `<h1>`** per page.
* Maintain proper heading hierarchy.
* Use headings semantically, not for styling.

---

# 📄 Paragraph Tag

Paragraphs are used to display blocks of textual information.

## Example

```html
<p>This is a paragraph.</p>
```

---

# 🔗 Hyperlinks

Hyperlinks connect webpages and external resources using the `<a>` tag.

## 📌 Example

```html
<a href="https://www.google.com">Visit Google</a>
```

---

# 🧠 Important Hyperlink Attributes

| Attribute         | Purpose                              |
| ----------------- | ------------------------------------ |
| `href`            | Defines the destination URL          |
| `target="_blank"` | Opens the link in a new tab          |
| `rel="noopener"`  | Improves security for external links |

---

# 🖼️ Images in HTML

Images are added using the `<img>` tag.

## 📌 Example

```html
<img src="image.jpg" alt="Sample Image" width="300">
```

---

# 🧠 Important Image Attributes

| Attribute          | Purpose                            |
| ------------------ | ---------------------------------- |
| `src`              | Image file path                    |
| `alt`              | Alternative text for accessibility |
| `width` & `height` | Controls image dimensions          |

---

# 📋 Ordered and Unordered Lists

Lists help organize information clearly.

---

# 🔹 Unordered List

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

## ✅ Output

* HTML
* CSS
* JavaScript

---

# 🔢 Ordered List

```html
<ol>
    <li>Install VS Code</li>
    <li>Create Project Folder</li>
    <li>Write HTML Code</li>
</ol>
```

## ✅ Output

1. Install VS Code
2. Create Project Folder
3. Write HTML Code

---

# 📊 Tables in HTML

Tables display structured data in rows and columns.

## 📌 Example

```html
<table border="1">

    <tr>
        <th>Name</th>
        <th>Role</th>
    </tr>

    <tr>
        <td>Utkarsh</td>
        <td>Developer</td>
    </tr>

</table>
```

---

# 🧠 Important Table Tags

| Tag       | Purpose         |
| --------- | --------------- |
| `<table>` | Creates a table |
| `<tr>`    | Table row       |
| `<th>`    | Table heading   |
| `<td>`    | Table data      |

---

# 🧾 Forms and Input Elements

Forms collect user information.

## 📌 Example

```html
<form>

    <label>Name:</label>
    <input type="text">

    <br><br>

    <label>Email:</label>
    <input type="email">

    <br><br>

    <button type="submit">Submit</button>

</form>
```

---

# 🏷️ Labels and Form Controls

Labels improve accessibility and usability.

## 📌 Example

```html
<label for="username">Username:</label>
<input type="text" id="username">
```

---

# 🧠 Semantic HTML Elements

Semantic elements provide meaning and structure to webpages.

## 📌 Examples

```html
<header></header>
<nav></nav>
<main></main>
<section></section>
<article></article>
<footer></footer>
```

---

# ✅ Benefits of Semantic HTML

* 🔍 Better SEO
* ♿ Improved accessibility
* 🧹 Cleaner code structure
* ⚙️ Easier maintenance
* 🌐 Better browser understanding

---

# 🎵 Audio Integration

HTML5 supports native audio playback.

## 📌 Example

```html
<audio controls>
    <source src="audio.mp3" type="audio/mp3">
</audio>
```

---

# 🎬 Video Integration

HTML5 supports video playback without external plugins.

## 📌 Example

```html
<video controls width="500">

    <source src="video.mp4" type="video/mp4">

</video>
```

---

# 🖥️ Embedding Content using iframe

The `<iframe>` tag embeds external webpages and services.

## 📌 Example

```html
<iframe 
    src="https://www.youtube.com"
    width="600"
    height="300">
</iframe>
```

---

# ⚡ Best Practices for HTML Development

* ✅ Write semantic HTML
* ✅ Maintain proper indentation
* ✅ Use meaningful tag names
* ✅ Add accessibility attributes
* ✅ Optimize images and media
* ✅ Validate HTML structure
* ✅ Avoid unnecessary nesting
* ✅ Follow responsive design principles

---

# 🛠️ Recommended Development Tools

| Tool                    | Purpose           |
| ----------------------- | ----------------- |
| 💻 VS Code              | Code Editor       |
| 🛠️ Chrome DevTools     | Debugging         |
| ⚡ Live Server Extension | Local Development |
| ✅ W3C Validator         | HTML Validation   |

---

# 🎯 Learning Outcomes

After completing this module, students will be able to:

* ✅ Understand frontend development fundamentals
* ✅ Build structured webpages using HTML5
* ✅ Create forms and tables
* ✅ Use semantic HTML correctly
* ✅ Integrate multimedia content
* ✅ Build accessible and SEO-friendly webpages
* ✅ Follow professional HTML development practices

---

# 📚 Conclusion

HTML is not just about displaying content — it provides:

* 📐 Structure
* 🌐 Meaning
* ♿ Accessibility
* 🔍 SEO optimization
* ⚡ Better browser communication

A strong understanding of HTML fundamentals is essential for becoming a professional frontend or full stack developer.

---

<div align="center">

### ⭐ Frontend Essentials Bootcamp 2026

### Built for Modern Web Development Learning

</div>
