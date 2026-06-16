# COM109 Week 4 – JavaScript Fundamentals

## Learning Outcomes

By the end of this session students should be able to:

- Understand the role of JavaScript in modern web applications
- Explain the relationship between HTML, CSS and JavaScript
- Understand the Document Object Model (DOM)
- Create and use variables
- Understand basic JavaScript data types
- Use arithmetic operators
- Display information using console.log()
- Respond to user events
- Understand the difference between let and const
- Understand the concept of variable scope

---

# Why This Week Matters

So far we have learned:

```text
HTML = Structure
CSS = Styling
```

This week we finally learn:

```text
JavaScript = Behaviour
```

JavaScript is what makes websites interactive.

Without JavaScript:

- Instagram cannot like posts
- Amazon cannot update baskets instantly
- Netflix menus cannot open dynamically
- Gmail cannot refresh content without reloading

Think of JavaScript as:

> The technology that makes websites respond to users.

---

# Class Opening (5 Minutes)

Walk in and ask:

### Question 1

What happens when you click "Like" on Instagram?

Students:

> It likes the post.

Then ask:

> Does HTML do that?

Answer:

> No.

---

### Question 2

What happens when Amazon updates your basket total instantly?

Students:

> It changes.

Ask:

> Is that CSS?

Answer:

> No.

---

### Question 3

What makes Netflix show a menu when you hover?

Students:

> JavaScript.

Then say:

> Today we learn the language that powers almost every modern website.

---

# Fun Facts

## Fun Fact 1

JavaScript runs on:

- Netflix
- Amazon
- YouTube
- Instagram
- TikTok
- Google Maps

Almost every modern website uses JavaScript.

---

## Fun Fact 2

JavaScript was created in only:

```text
10 days
```

by Brendan Eich in 1995.

---

## Fun Fact 3

JavaScript and Java are completely different technologies.

```text
Java ≠ JavaScript
```

The names sound similar but they are different programming languages.

---

# The Big Picture

Draw this diagram:

```text
Website

HTML
|
Structure

CSS
|
Styling

JavaScript
|
Behaviour
```

---

# Real World Analogy

```text
Car

Body
=
HTML

Paint
=
CSS

Engine
=
JavaScript
```

Without the engine, the car looks nice but does not do anything useful.

---

# Section 1 – What is JavaScript?

## Simple Explanation

JavaScript allows websites to:

- React
- Calculate
- Update
- Validate
- Interact

---

## Real World Examples

### Instagram

```text
Like Button
```

Powered by JavaScript.

---

### Amazon

```text
Basket Total Updates
```

Powered by JavaScript.

---

### Netflix

```text
Recommendations
```

Powered by JavaScript.

---

### Gmail

```text
Refresh Inbox Without Reloading
```

Powered by JavaScript.

---

## Question for Students

Can HTML perform any of these tasks by itself?

Answer:

> No.

---

# Section 2 – Client-Side vs Server-Side JavaScript

## Client Side

Runs inside the browser.

```text
Browser
|
JavaScript
|
Runs Here
```

Example:

```text
Password Length Validation
```

The browser checks immediately.

---

## Server Side

Runs on a server.

```text
Browser
|
Server
|
JavaScript (Node.js)
```

Example:

```text
Login Verification
```

The server verifies credentials.

---

# Section 3 – The DOM (Document Object Model)

## What is the DOM?

The DOM is the browser's internal representation of a webpage.

Think of it as:

> A map of the webpage.

---

## DOM Structure

```text
html

|
+-- head

|
+-- body

    |
    +-- h1

    |
    +-- p

    |
    +-- button
```

---

## Real World Analogy

```text
Website = House

DOM = House Blueprint
```

The DOM shows where everything is located.

---

## JavaScript and DOM

JavaScript uses the DOM to find and change elements.

Example:

```javascript
document.getElementById("title")
```

Meaning:

> Find the element with the ID "title".

---

## Student Question

If JavaScript cannot find a button, can it change the button?

Answer:

> No.

---

# Section 4 – Objects

Everything in JavaScript is based around objects.

---

## Phone Example

### Properties

```text
Colour
Size
Brand
```

---

### Methods

```text
Call()
Text()
```

---

## Button Example

### Properties

```text
Text
Colour
Size
```

---

### Methods

```text
Click()
Focus()
```

---

# Section 5 – Events

## What is an Event?

An event is something that happens on a webpage.

Examples:

- Mouse click
- Key press
- Page load
- Mouse hover

---

## Event Flow

```text
User Clicks

↓

Event

↓

JavaScript Runs

↓

Action Happens
```

---

## Example

```html
<button onclick="sayHello()">
Click Me
</button>
```

---

## Real World Examples

| Event | Website Example |
|---------|---------|
| Click | Add To Cart |
| Hover | Netflix Menu |
| KeyPress | Search Box |
| Load | Homepage Loading |
| Resize | Responsive Design |

---

# Live Demo 1

```html
<button onclick="alert('Hello')">
Click Me
</button>
```

---

# Section 6 – Variables

## What is a Variable?

A variable is a container that stores information.

---

## Real World Analogy

```text
Name Box

[Vishnu]
```

---

## Example

```javascript
let name = "Vishnu";
```

---

### Age

```javascript
let age = 27;
```

---

### Bank Balance

```javascript
let balance = 1500;
```

---

## Real World Examples

### Instagram

```javascript
let likes = 500;
```

---

### Amazon

```javascript
let basketTotal = 99.99;
```

---

## Student Question

What variables might Netflix use?

Examples:

```javascript
let movieTitle;
let userName;
```

---

# Section 7 – Data Types

## Number

```javascript
let age = 27;
```

---

## String

```javascript
let name = "John";
```

---

## Boolean

```javascript
let loggedIn = true;
```

---

## NaN

Means:

```text
Not a Number
```

Occurs when JavaScript cannot perform a valid numeric calculation.

---

# Section 8 – Operators

## Addition

```javascript
5 + 5
```

---

## Subtraction

```javascript
10 - 5
```

---

## Multiplication

```javascript
10 * 5
```

---

## Division

```javascript
10 / 5
```

---

## Modulus (Remainder)

```javascript
15 % 9
```

Result:

```javascript
6
```

---

## Real World Example

```javascript
basketTotal + deliveryCharge
```

Used in ecommerce websites.

---

# Section 9 – Console

## What is the Console?

The console is where developers communicate with the browser.

---

## Open Console

```text
Right Click
↓

Inspect
↓

Console
```

---

## Example

```javascript
console.log("Hello");
```

---

## Example 2

```javascript
let age = 27;

console.log(age);
```

---

# Section 10 – let vs const

## let

Can be changed.

```javascript
let score = 10;

score = 20;
```

---

## const

Cannot be changed.

```javascript
const pi = 3.14;
```

---

## Real World Example

```javascript
const university = "QA";
```

The university name remains constant.

---

# Section 11 – Scope

## Simple Explanation

Scope determines where a variable can be accessed.

---

## Local Scope

Accessible only within a function.

---

## Global Scope

Accessible throughout the program.

---

## Real World Analogy

```text
Local Scope

Your Bedroom

Global Scope

Entire House
```

---

# Live Coding Session

## Demo 1

```html
<button onclick="sayHello()">
Click Me
</button>

<script>

function sayHello() {
    alert("Hello COM109");
}

</script>
```

---

## Demo 2

```javascript
let age = 20;

console.log(age);
```

---

## Demo 3

```javascript
let x = 10;
let y = 5;

console.log(x + y);
```

---

## Demo 4

```javascript
let likes = 0;

function addLike() {

    likes++;

    console.log(likes);

}
```

Students love watching the counter increase.

---

# Seminar Introduction

Today's practical focuses on:

```text
Variables
↓

Operators
↓

Console

↓

Events

↓

Debugging
```

You will create JavaScript variables, perform calculations, handle events and fix common JavaScript errors.

---

# Key Concepts To Remember

If you understand these concepts, you have mastered the foundations of JavaScript:

1. What JavaScript is
2. DOM
3. Events
4. Variables
5. Data Types
6. Operators
7. Console.log()
8. let vs const

These concepts form the foundation for:

- Functions
- Arrays
- Loops
- Objects
- jQuery
- React
- Angular
- Modern Web Development

---

# End of Lecture Summary

Today we learned:

```text
HTML
=
Structure

CSS
=
Styling

JavaScript
=
Behaviour
```

JavaScript is what transforms a static webpage into an interactive web application.

Every modern website uses JavaScript to respond to users, update content and create engaging experiences.
