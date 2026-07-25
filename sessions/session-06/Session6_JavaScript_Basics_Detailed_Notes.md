# Session 6 – JavaScript Basics (Detailed Notes)

> These notes are based on the provided Session 6 PDF and expand each topic with explanations and additional code examples for students. Source: fileciteturn0file0

# Table of Contents

1. Introduction to JavaScript
2. Adding JavaScript to HTML
3. Variables and Constants
4. Data Types
5. Operators
6. Conditional Statements
7. switch Statement
8. Loops
9. Real World Grade Calculator
10. Best Practices
11. Common Mistakes
12. Practice Questions

---

# 1. Introduction to JavaScript

## What is JavaScript?

JavaScript (JS) is a programming language that adds **behavior** and **interactivity** to web pages.

HTML = Structure

CSS = Styling

JavaScript = Logic + Interaction

Examples:
- Button Click
- Form Validation
- Image Slider
- Calculator
- Games
- Dynamic Content

```js
console.log("Hello JavaScript");
```

---

# 2. Adding JavaScript to HTML

## 1. Inline JavaScript (Avoid)

```html
<button onclick="alert('Hello')">Click</button>
```

## 2. Internal JavaScript

```html
<script>
console.log("Internal JS");
</script>
```

## 3. External JavaScript (Recommended)

```html
<script src="script.js"></script>
```

Create:

```text
index.html
script.js
```

```js
console.log("External JS File");
```

Why External?

- Easy Maintenance
- Reusable
- Clean HTML
- Professional Standard

---

# 3. Variables and Constants

Variables store data.

## let

```js
let age = 20;
age = 21;
```

Can be reassigned.

## const

```js
const country = "India";
```

Cannot be reassigned.

## var (Legacy)

```js
var x = 10;
```

Avoid in modern JavaScript.

## Naming Rules

✅ studentName

✅ totalPrice

❌ 1name

❌ my-name

Use camelCase.

---

# 4. Data Types

## String

```js
let name = "Utkarsh";
```

## Number

```js
let age = 21;
let price = 499.99;
```

## Boolean

```js
let isStudent = true;
```

## Undefined

```js
let city;
```

## Null

```js
let user = null;
```

## typeof

```js
console.log(typeof age);
console.log(typeof name);
console.log(typeof isStudent);
```

---

# 5. Operators

## Arithmetic

```js
let a = 10;
let b = 3;

console.log(a+b);
console.log(a-b);
console.log(a*b);
console.log(a/b);
console.log(a%b);
console.log(a**b);
```

## Assignment

```js
let x = 5;

x += 2;
x -= 1;
x *= 3;
x /= 2;
```

## Comparison

```js
10 > 5
10 < 5
10 >= 5
10 <= 5
10 === 10
10 !== 5
```

Always use:

```js
===
!==
```

instead of

```js
==
!=
```

## Logical

```js
true && false
true || false
!true
```

Example

```js
let age = 20;
let hasID = true;

if(age>=18 && hasID){
    console.log("Allowed");
}
```

---

# 6. Conditional Statements

## if

```js
let age=20;

if(age>=18){
 console.log("Adult");
}
```

## if else

```js
if(age>=18){
 console.log("Adult");
}
else{
 console.log("Minor");
}
```

## if else if else

```js
let marks=75;

if(marks>=90){
 console.log("A");
}
else if(marks>=75){
 console.log("B");
}
else if(marks>=60){
 console.log("C");
}
else{
 console.log("Fail");
}
```

Rules

- Checked from top to bottom
- First true block executes
- Remaining blocks skipped

---

# 7. switch Statement

```js
let day="Mon";

switch(day){

case "Mon":
console.log("Bootcamp");
break;

case "Tue":
console.log("Tuesday");
break;

default:
console.log("Holiday");

}
```

Remember:
- break prevents fall-through.
- default runs when no case matches.

---

# 8. Loops

## for Loop

```js
for(let i=1;i<=5;i++){
 console.log(i);
}
```

Even Numbers

```js
for(let i=1;i<=10;i++){
 if(i%2===0){
   console.log(i);
 }
}
```

## while Loop

```js
let i=1;

while(i<=5){
 console.log(i);
 i++;
}
```

## do while Loop

```js
let i=1;

do{
 console.log(i);
 i++;
}while(i<=5);
```

Difference

| while | do while |
|---------|-----------|
|Checks first|Runs once before checking|

---

# 9. Real World Example

```js
const marksList=[85,42,67,90,55];

for(let i=0;i<marksList.length;i++){

 let marks=marksList[i];
 let grade;

 if(marks>=75){
   grade="A";
 }
 else if(marks>=50){
   grade="B";
 }
 else{
   grade="Fail";
 }

 console.log(`Student ${i+1}: ${grade}`);

}
```

Concepts Used

- const
- let
- arrays
- loop
- if else
- template literals

---

# 10. Best Practices

- Prefer const by default.
- Use let only when values change.
- Never use var in modern code.
- Use descriptive variable names.
- Always use === and !==.
- Keep code properly indented.
- Comment complex logic.

---

# 11. Common Mistakes

❌ Forgetting break in switch

❌ Infinite loops

```js
while(true){

}
```

❌ Using ==

```js
"5" == 5
```

Use

```js
"5" === 5
```

❌ Poor variable names

```js
let a=10;
```

Better

```js
let studentAge=10;
```

---

# 12. Practice Questions

1. Print your name using console.log().
2. Create variables using let and const.
3. Find the datatype of five values.
4. Perform all arithmetic operations.
5. Check whether a number is even or odd.
6. Find the largest of two numbers.
7. Build a Grade Calculator.
8. Print numbers 1–20 using for loop.
9. Print even numbers from 1–100.
10. Print odd numbers from 1–100.
11. Print multiplication table of any number.
12. Print numbers using while loop.
13. Print numbers using do-while loop.
14. Use switch to print weekday.
15. Create an array of five numbers and print each using a loop.

---

# Summary

Students should now understand:

- JavaScript basics
- Variables
- Data Types
- Operators
- Decision Making
- switch
- Loops
- Real-world examples
- Coding Best Practices

Practice every concept by writing code instead of only reading.
