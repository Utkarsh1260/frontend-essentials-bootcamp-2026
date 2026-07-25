# Session 7 — JavaScript Interactivity & DOM Basics



---

## 🎯 Learning Outcome

By the end of this session, you will be able to:

- Write and call **functions** to organize reusable logic
- Work with **arrays** to store and loop through data
- Navigate the **DOM** to find any element on a page
- Handle **user events** like clicks, typing, and form submits
- Update a page **live** by changing text, style, and content
- Build a small **interactive UI** combining everything above

> *"Add basic interactivity and dynamic behavior to web pages."*

---

## 📋 Topics Covered Today

| # | Topic | What it's about |
|---|-------|------------------|
| 1 | Functions | Reusable blocks of logic |
| 2 | Arrays | Storing and looping through lists of data |
| 3 | Introduction to the DOM | What the DOM is, how the browser builds it |
| 4 | DOM Selection & Manipulation | Selecting elements and changing them |
| 5 | Events & Event Handling | Reacting to what the user does |
| 6 | Interactive Web Elements | Combining everything into one mini project |

---

## 1️⃣ Functions — Reusable Blocks of Logic

A **function** packages a piece of code so you can run it again and again without rewriting it. Instead of copy-pasting the same logic everywhere, you write it once and *call* it whenever needed.

### Key Points
- Declared with `function name(params) { ... }`
- **Arrow functions** are a shorter way to write functions: `const name = () => { ... }`
- `return` sends a value back to wherever the function was called — without `return`, a function gives back `undefined`
- Parameters are placeholders for values you pass in when calling the function

### Code Example

```javascript
// function declaration
function greetStudent(name) {
  return `Hello, ${name}! 👋`;
}

// arrow function
const add = (a, b) => a + b;

console.log(greetStudent("Utkarsh")); // "Hello, Utkarsh! 👋"
console.log(add(5, 3));               // 8
```

### 💡 Real-World Example

An e-commerce site uses a `calculateTotal(cartItems)` function every single time you add or remove a product — instead of rewriting the price-adding logic on every button.

```javascript
function calculateTotal(cart) {
  let total = 0;
  for (let item of cart) {
    total += item.price * item.qty;
  }
  return total;
}

calculateTotal(cart); // ₹2,450
```

### 🧠 Why it matters
Every time you see repeated logic in your code, that's a sign it should become a function. This keeps your code short, readable, and easy to fix (change it in one place, not ten).

---

## 2️⃣ Arrays — Storing Lists of Data

An **array** holds an ordered list of values inside a single variable. Think of it as a numbered row of boxes, where each box holds one value.

### Key Points
- Access items by **index**: `arr[0]` is the first item, `arr[1]` the second, and so on
- Arrays are zero-indexed — counting starts from `0`, not `1`
- Loop through arrays with `for`, `for...of`, or `.forEach()`
- Common built-in methods:
  - `.push(value)` — add an item to the end
  - `.pop()` — remove the last item
  - `.map(fn)` — create a new array by transforming each item
  - `.filter(fn)` — create a new array keeping only items that pass a condition

### Code Example

```javascript
const students = ["Aman", "Riya", "Sam"];

students.push("Neha");
console.log(students[0]);  // "Aman"

students.forEach((s) => {
  console.log(`Hi ${s}`);
});
```

### 💡 Real-World Example

A to-do list app stores every task inside a `tasks` array. Adding a task pushes to it, completing one filters it out — the array is the single source of truth for what renders on screen.

```javascript
let tasks = ["Learn DOM", "Build UI"];

// add a new task
tasks.push("Submit assignment");

// remove a completed task
tasks = tasks.filter(
  (t) => t !== "Learn DOM"
);
```

### 🧠 Why it matters
Almost every dynamic list you see on the web — notifications, cart items, search results, chat messages — is powered by an array behind the scenes.

---

## 3️⃣ Introduction to the DOM

**DOM** stands for **Document Object Model** — it's the browser's live, tree-shaped representation of your HTML that JavaScript can read and change.

### Key Points
- **It's a tree** — every HTML tag becomes a connected "node" in that tree
- **The browser builds it automatically** the moment a page loads, from your HTML file
- **JavaScript can change it live** — no page reload needed, updates happen instantly on screen

### Visualizing the Tree

```
<html>
 ├── <head>
 └── <body>
      ├── <h1>  →  "Bootcamp"
      └── <button>
```

Every box in that tree is a **node**. JavaScript can select any node and read or change what's inside it, live in the browser — that's the foundation of everything that follows in this session.

### 🧠 Why it matters
The DOM is *the* bridge between your HTML and your JavaScript. Without understanding the DOM, you can't make a page interactive — you're just writing static HTML.

---

## 4️⃣ DOM Selection & Manipulation

Now that we understand the DOM is a tree of nodes, let's learn how to **grab** a node and **change** it.

### Key Points
- `document.querySelector(".class")` — grabs the **first** element matching that selector
- `document.querySelectorAll("li")` — grabs **all** matching elements as a list (NodeList)
- `.textContent` / `.innerHTML` — read or change the text/HTML inside an element
- `.style.property` — change CSS directly from JavaScript
- `.classList.add() / .remove() / .toggle()` — control CSS classes dynamically

### Code Example

```javascript
const title = document.querySelector("h1");

title.textContent = "Welcome!";
title.style.color = "#2DD4BF";
```

### 💡 Real-World Example

A dark-mode toggle on a website selects the `<body>` element and swaps its class — every color on the page updates instantly, no reload needed.

```javascript
const body = document.body;
const btn = document.querySelector("#themeBtn");

btn.addEventListener("click", () => {
  body.classList.toggle("dark");
});

// CSS
// .dark { background: #0B1120; }
```

### 🧠 Why it matters
Selection is how JavaScript "finds" the exact part of the page you want to work with. Manipulation is how it "changes" that part. Together, these two skills are what let JS bring a static page to life.

---

## 5️⃣ Events & Event Handling

An **event** is anything the user does on a page — clicking, typing, scrolling, submitting a form. JavaScript can **listen** for these events and react to them.

### Key Points
- `element.addEventListener("click", handlerFn)` listens for an event on an element
- The handler function runs **automatically** whenever that event fires — you never call it yourself
- Common event types: `"click"`, `"input"`, `"submit"`, `"keydown"`, `"mouseover"`
- `event.preventDefault()` stops a form's default behavior (like reloading the page on submit)

### Code Example

```javascript
const btn = document.querySelector("#likeBtn");

btn.addEventListener("click", () => {
  console.log("Button clicked!");
});
```

### 💡 Real-World Example

Instagram's like button listens for a `click` event, instantly turns red, and updates the like count — all through one event listener.

```javascript
const form = document.querySelector("#loginForm");

form.addEventListener("submit", (e) => {
  e.preventDefault();
  console.log("Form submitted!");
});
```

### 🧠 Why it matters
Events are what make a page *interactive* rather than just *readable*. Every button click, form submission, and hover effect you've ever used on the web runs through an event listener.

---

## 6️⃣ Interactive Web Elements — Putting It All Together

This is where **Functions + Arrays + DOM + Events** combine into one real interactive feature. Let's break down a simple task counter that adds items to a list on the page.

### Full Code Example

```javascript
let tasks = [];

const list = document.querySelector("#taskList");
const input = document.querySelector("#taskInput");
const addBtn = document.querySelector("#addBtn");

function renderTasks() {
  list.innerHTML = "";
  tasks.forEach((task) => {
    const li = document.createElement("li");
    li.textContent = task;
    list.appendChild(li);
  });
}

addBtn.addEventListener("click", () => {
  tasks.push(input.value);
  renderTasks();
  input.value = "";
});
```

### What's Happening Here?

| Piece | Role |
|-------|------|
| **Array** (`tasks[]`) | Stores every task the user adds |
| **DOM Selection** (`querySelector`) | Grabs the input, button, and list from the page |
| **Function** (`renderTasks()`) | Redraws the list every time something changes |
| **Event** (`addEventListener`) | A click triggers the entire update chain |

> 🔑 **This exact pattern powers to-do apps, cart counters, and like buttons across the real web.**

### Bonus Example — Changing Text & Color on Click

```javascript
// Select Elements
const heading = document.querySelector("#heading");
const box = document.querySelector("#box");
const button = document.querySelector("#btn");

// Button Click Event
button.addEventListener("click", () => {
  // Change the text
  heading.textContent = "Welcome to JavaScript DOM!";

  // Change the color of the box
  box.style.backgroundColor = "tomato";
});
```

---

## ✅ Recap — Key Takeaways

- **Functions** — Package reusable logic with `function` or arrow syntax
- **Arrays** — Store and loop through lists of data with built-in methods
- **The DOM** — The tree-structure the browser builds from your HTML
- **Selection** — `querySelector()` / `querySelectorAll()` find any element
- **Manipulation** — Change text, styles & classes to update the page live
- **Events** — `addEventListener()` reacts to clicks, input & submits

---

## 📝 Practice Before Next Session

Try building these on your own using today's concepts:

1. A button that changes a heading's text and background color on click (see Bonus Example above)
2. A simple to-do list where you can add and remove tasks (see the task counter example)
3. A dark-mode toggle for a basic HTML page
4. A form that logs the entered value to the console instead of reloading the page

---

*Questions? Drop them in the Discord channel — see you in Session 8, where we'll build further on today's DOM & event-handling skills.*
