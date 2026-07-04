# Advanced HTML & Forms Complete Notes

## Tables • Forms • Inputs • Semantic HTML • Multimedia • iframe

> Based on the uploaded Session 2 PDF — *Advanced HTML & Forms* 

---

# Table of Contents

1. Introduction to Advanced HTML
2. Understanding HTML Tables
3. Table Tags Explained
4. Creating Basic Tables
5. Advanced Table Features
6. Introduction to HTML Forms
7. Form Structure in HTML
8. Input Types in HTML
9. Text, Email & Password Inputs
10. Radio Buttons & Checkboxes
11. Dropdown Menus & Textarea
12. Labels & Form Controls
13. Student Registration Form Project
14. Semantic HTML
15. Semantic vs Non-Semantic Tags
16. Semantic Layout Structure
17. Audio in HTML
18. Video in HTML
19. iframe in HTML
20. HTML Best Practices
21. Common Beginner Mistakes
22. Final Thoughts

---

# 1. Introduction to Advanced HTML

HTML is the foundation of every webpage.

Basic HTML helps us create:

* headings
* paragraphs
* lists
* images
* links

Advanced HTML helps us build:

* forms
* tables
* multimedia webpages
* structured layouts
* interactive webpages

---

# Why Advanced HTML is Important

Modern websites require:

* data collection
* structured content
* multimedia support
* semantic structure
* accessibility

Examples:

* login pages
* registration forms
* dashboards
* blogs
* video platforms

---

# Real-World Websites Using Advanced HTML

* Google
* Facebook
* YouTube
* Amazon

All heavily use:

* forms
* tables
* semantic structure
* multimedia

---

# 2. Understanding HTML Tables

The uploaded PDF explains tables in detail. 

HTML tables organize data into:

* rows
* columns

---

# Real-World Examples of Tables

Tables are used in:

* student marksheets
* invoices
* schedules
* reports
* dashboards

---

# Structure of a Table

```text id="j1"
TABLE
 ├── ROWS
 │    ├── COLUMNS
 │    ├── DATA
```

---

# Main Table Tags

| Tag       | Purpose       |
| --------- | ------------- |
| `<table>` | Creates table |
| `<tr>`    | Table row     |
| `<th>`    | Table heading |
| `<td>`    | Table data    |

---

# 3. Table Tags Explained

---

# `<table>`

Container for complete table.

---

# Example

```html id="j2"
<table>

</table>
```

---

# `<tr>` — Table Row

Defines horizontal row.

---

# Example

```html id="j3"
<tr>

</tr>
```

---

# `<th>` — Table Header

Creates bold heading cells.

---

# Example

```html id="j4"
<th>Name</th>
```

---

# `<td>` — Table Data

Stores actual content.

---

# Example

```html id="j5"
<td>Rahul</td>
```

---

# 4. Creating Basic Tables

The PDF provides a table example. 

---

# Complete Example

```html id="j6"
<table border="1">

  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>

  <tr>
    <td>Rahul</td>
    <td>20</td>
    <td>Jabalpur</td>
  </tr>

  <tr>
    <td>Priya</td>
    <td>21</td>
    <td>Indore</td>
  </tr>

</table>
```

---

# Output Structure

| Name  | Age | City     |
| ----- | --- | -------- |
| Rahul | 20  | Jabalpur |
| Priya | 21  | Indore   |

---

# Understanding border Attribute

```html id="j7"
border="1"
```

Adds visible borders.

---

# Important Concept

Each row:

```html id="j8"
<tr>
```

Contains:

```html id="j9"
<td>
```

or:

```html id="j10"
<th>
```

---

# 5. Advanced Table Features

The PDF introduces advanced table attributes. 

---

# colspan

Merges columns horizontally.

---

# Example

```html id="j11"
<td colspan="2">
  Total
</td>
```

---

# rowspan

Merges rows vertically.

---

# Example

```html id="j12"
<td rowspan="2">
  Score
</td>
```

---

# cellpadding

Adds spacing INSIDE cells.

---

# Example

```html id="j13"
<table cellpadding="10">
```

---

# cellspacing

Adds spacing BETWEEN cells.

---

# Example

```html id="j14"
<table cellspacing="5">
```

---

# Complete Advanced Table

```html id="j15"
<table border="1" cellpadding="10">

  <tr>
    <th>Name</th>
    <th colspan="2">Marks</th>
  </tr>

  <tr>
    <td>Rahul</td>
    <td>80</td>
    <td>90</td>
  </tr>

</table>
```

---

# 6. Introduction to HTML Forms

The PDF explains forms thoroughly. 

Forms collect user input.

---

# Real-World Examples

Forms are used for:

* login
* signup
* contact forms
* payment pages
* surveys

---

# Basic Form Structure

```html id="j16"
<form>

</form>
```

---

# Form with action and method

```html id="j17"
<form action="submit.php" method="POST">

</form>
```

---

# action Attribute

Defines:

* where form data goes

---

# method Attribute

Defines:

* how data is sent

---

# GET vs POST

| Method | Purpose           |
| ------ | ----------------- |
| GET    | Sends data in URL |
| POST   | Sends secure data |

---

# 7. Form Structure in HTML

The PDF explains the structure well. 

---

# Example Form

```html id="j18"
<form>

  <label>Name:</label>
  <input type="text">

  <br><br>

  <label>Email:</label>
  <input type="email">

  <br><br>

  <input type="submit">

</form>
```

---

# Important Elements

| Tag        | Purpose           |
| ---------- | ----------------- |
| `<form>`   | Form container    |
| `<label>`  | Input description |
| `<input>`  | User input        |
| `<submit>` | Sends form        |

---

# placeholder Attribute

Shows temporary hint text.

---

# Example

```html id="j19"
<input type="text"
placeholder="Enter your name">
```

---

# 8. Input Types in HTML

The PDF includes major input types. 

---

# Common Input Types

| Type     | Purpose            |
| -------- | ------------------ |
| text     | Text input         |
| email    | Email validation   |
| password | Hidden characters  |
| number   | Numeric values     |
| radio    | One selection      |
| checkbox | Multiple selection |
| file     | Upload files       |
| submit   | Submit form        |

---

# 9. Text, Email & Password Inputs

The PDF explains these clearly. 

---

# Text Input

```html id="j20"
<input type="text"
placeholder="Enter name">
```

Accepts normal text.

---

# Email Input

```html id="j21"
<input type="email"
placeholder="user@example.com">
```

Performs email validation.

---

# Password Input

```html id="j22"
<input type="password"
placeholder="Enter password">
```

Hides typed characters.

---

# Why Validation Matters

Validation improves:

* security
* user experience
* correct data submission

---

# 10. Radio Buttons & Checkboxes

The PDF explains the difference well. 

---

# Radio Buttons

Used when ONLY ONE option allowed.

---

# Example

```html id="j23"
<input type="radio" name="gender">
Male

<input type="radio" name="gender">
Female
```

---

# Important Rule

All radio buttons in same group MUST share same:

```html id="j24"
name
```

---

# Checkboxes

Used when MULTIPLE options allowed.

---

# Example

```html id="j25"
<input type="checkbox">
Java

<input type="checkbox">
Python
```

---

# Difference Between Radio & Checkbox

| Radio          | Checkbox         |
| -------------- | ---------------- |
| Single choice  | Multiple choices |
| Linked by name | Independent      |

---

# 11. Dropdown Menus & Textarea

The PDF discusses dropdowns and textarea. 

---

# Dropdown Menu

Created using:

```html id="j26"
<select>
```

---

# Example

```html id="j27"
<select>

  <option>India</option>
  <option>USA</option>
  <option>UK</option>

</select>
```

---

# option Tag

Represents each choice.

---

# textarea

Creates multi-line input.

---

# Example

```html id="j28"
<textarea rows="4" cols="40">

</textarea>
```

---

# Real-World Usage

textarea used for:

* comments
* feedback
* messages
* descriptions

---

# 12. Labels & Form Controls

The PDF emphasizes accessibility importance. 

---

# Why Labels Matter

Benefits:

* accessibility
* better UX
* easy clicking
* screen reader support

---

# Incorrect Practice

```html id="j29"
<input type="text">
```

No label.

---

# Correct Practice

```html id="j30"
<label for="username">
  Username
</label>

<input type="text" id="username">
```

---

# Important Rule

```text id="j31"
for attribute MUST match id
```

---

# Benefits of Labels

---

## 1. Accessibility

Screen readers understand forms better.

---

## 2. Better UX

Users know field purpose instantly.

---

## 3. Easy Clicking

Clicking label focuses input.

---

# 13. Student Registration Form Project

The PDF contains a mini project. 

---

# Complete Project

```html id="j32"
<form>

  <label for="name">
    Name:
  </label>

  <input type="text" id="name">

  <br><br>

  <label for="email">
    Email:
  </label>

  <input type="email" id="email">

  <br><br>

  <label for="course">
    Course:
  </label>

  <select id="course">

    <option>BCA</option>
    <option>B.Tech</option>
    <option>MCA</option>

  </select>

  <br><br>

  <label>Gender:</label>

  <input type="radio" name="g">
  Male

  <input type="radio" name="g">
  Female

  <br><br>

  <label>Interests:</label>

  <input type="checkbox">
  Web Dev

  <input type="checkbox">
  AI/ML

  <br><br>

  <input type="submit"
  value="Register">

</form>
```

---

# Concepts Used

* text input
* email input
* select dropdown
* radio buttons
* checkboxes
* submit button

---

# 14. Semantic HTML

Semantic HTML gives meaning to webpage structure.

The PDF explains semantic HTML deeply. 

---

# What is Semantic HTML?

Semantic tags describe:

* purpose
* meaning
* content type

---

# Examples

| Semantic Tag | Purpose             |
| ------------ | ------------------- |
| header       | Top section         |
| nav          | Navigation          |
| main         | Main content        |
| section      | Section block       |
| article      | Independent article |
| aside        | Sidebar             |
| footer       | Bottom section      |

---

# 15. Semantic vs Non-Semantic Tags

The PDF compares semantic and non-semantic tags. 

---

# Semantic Tags

```html id="j33"
<header>
<nav>
<section>
<footer>
```

Clearly describe meaning.

---

# Non-Semantic Tags

```html id="j34"
<div>
<span>
```

No meaning by themselves.

---

# Why Semantic HTML Matters

Benefits:

* better SEO
* accessibility
* readable code
* maintainability

---

# 16. Semantic Layout Structure

The PDF provides semantic structure example. 

---

# Complete Example

```html id="j35"
<header>

  <h1>My Portfolio</h1>

</header>

<nav>

  <a href="#">Home</a>
  <a href="#">About</a>

</nav>

<main>

  <section>

    <h2>About Me</h2>

    <p>
      I am a developer.
    </p>

  </section>

  <article>

    <h2>Blog Post</h2>

    <p>
      Article content.
    </p>

  </article>

</main>

<footer>

  <p>
    Copyright 2026
  </p>

</footer>
```

---

# Advantages

---

## Better SEO

Search engines understand structure.

---

## Better Accessibility

Screen readers navigate easily.

---

## Better Maintainability

Code becomes cleaner.

---

# 17. Audio in HTML

The PDF explains audio embedding. 

---

# Audio Tag

```html id="j36"
<audio controls>

  <source
  src="music.mp3"
  type="audio/mpeg">

</audio>
```

---

# controls Attribute

Shows:

* play
* pause
* volume

---

# Other Audio Attributes

| Attribute | Purpose              |
| --------- | -------------------- |
| autoplay  | Starts automatically |
| loop      | Repeats audio        |
| muted     | Starts muted         |

---

# 18. Video in HTML

---

# Video Example

```html id="j37"
<video controls
width="400"
height="250">

  <source
  src="movie.mp4"
  type="video/mp4">

</video>
```

---

# Important Attributes

| Attribute | Purpose        |
| --------- | -------------- |
| controls  | Video controls |
| autoplay  | Auto play      |
| loop      | Repeat         |
| muted     | Muted start    |
| width     | Width          |
| height    | Height         |

---

# 19. iframe in HTML

The PDF discusses iframe embedding. 

---

# What is iframe?

iframe embeds another webpage inside webpage.

---

# Basic iframe

```html id="j38"
<iframe
src="https://example.com"
width="600"
height="400">
</iframe>
```

---

# YouTube Embed

```html id="j39"
<iframe
src="https://www.youtube.com/embed/VIDEO_ID"
width="560"
height="315"
allowfullscreen>
</iframe>
```

---

# Google Maps Embed

```html id="j40"
<iframe
src="https://maps.google.com/maps?q=Jabalpur"
width="600"
height="450">
</iframe>
```

---

# Real-World Uses

iframe used for:

* YouTube videos
* Google Maps
* Ads
* Widgets
* External websites

---

# 20. HTML Best Practices

The PDF provides professional practices. 

---

# 1. Use Semantic Tags

Prefer:

```html id="j41"
<header>
<section>
<footer>
```

Instead of:

```html id="j42"
<div>
```

everywhere.

---

# 2. Write Clean Code

Use proper indentation.

---

# Bad

```html id="j43"
<div><p>Hello</p></div>
```

---

# Good

```html id="j44"
<div>

  <p>Hello</p>

</div>
```

---

# 3. Always Use Labels

Better accessibility.

---

# 4. Use Meaningful Names

✅ Good:

```html id="j45"
id="studentName"
```

❌ Bad:

```html id="j46"
id="s1"
```

---

# 5. Validate Forms Properly

Use:

* required
* email validation
* proper input types

---

# 21. Common Beginner Mistakes

---

# Mistake 1: Using Tables for Layout

Tables should organize data only.

---

# Mistake 2: Missing Labels

Hurts accessibility.

---

# Mistake 3: Wrong Input Types

Example:

```html id="j47"
type="text"
```

Instead of:

```html id="j48"
type="email"
```

---

# Mistake 4: Excessive div Usage

Prefer semantic tags.

---

# Mistake 5: Poor Indentation

Makes debugging difficult.

---

# 22. Final Thoughts

Advanced HTML is essential for:

* professional webpages
* forms
* structured layouts
* multimedia integration
* accessible websites

By mastering:

* tables
* forms
* semantic HTML
* multimedia
* iframe

You can build:

* real-world websites
* interactive applications
* professional UI structures

---

# What to Practice Next

Build:

* registration forms
* login forms
* timetable tables
* portfolio layouts
* blog structures

---

# Recommended Next Topics

After Advanced HTML learn:

* CSS Fundamentals
* Flexbox
* Grid
* Responsive Design
* JavaScript DOM

---

# Practice Challenge

Build:

1. Student Registration Form
2. Resume Layout
3. Portfolio Webpage
4. YouTube Video Embed Page
5. Contact Form with Semantic Layout

---

# Key Takeaway

> HTML creates the structure of the web.
> Advanced HTML creates interactive, meaningful, and accessible webpages.

---

Happy Coding 🚀
