# COM109 Week 4 – JavaScript Fundamentals

## Learning Outcomes

By the end of this session, students should be able to:

* Explain the purpose of JavaScript in modern websites
* Understand how JavaScript works alongside HTML and CSS
* Use the browser console
* Create and use variables
* Understand basic data types
* Perform calculations using operators
* Create and call functions
* Respond to user interactions
* Understand the basics of the DOM

---

# Why This Week Matters

So far we have learned:

```text
HTML = Structure
CSS = Styling
```

Today we learn:

```text
JavaScript = Behaviour
```

Without JavaScript:

* Instagram cannot like posts
* Amazon cannot update basket totals instantly
* Netflix menus cannot open dynamically
* Google Maps cannot respond to user actions
* Gmail cannot refresh messages without reloading

Think of JavaScript as:

> The technology that makes websites respond to users.

---

# Technical Fun Facts

### Fun Fact 1

JavaScript was created in only **10 days** by Brendan Eich in 1995.

---

### Fun Fact 2

JavaScript runs on:

* Netflix
* Amazon
* TikTok
* YouTube
* Instagram
* Google Maps
* Facebook

Almost every modern website uses JavaScript.

---

### Fun Fact 3

JavaScript and Java are completely different.

```text
Java ≠ JavaScript
```

The names are similar, but they are different technologies.

---

### Fun Fact 4

Over 98% of websites use JavaScript.

That means almost every website your students visit daily uses JavaScript.

---

# Big Picture

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

Imagine a car.

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

Without an engine, the car looks nice but cannot move.

Without JavaScript, a webpage looks nice but cannot respond to users.

---

# Teaching Order

For beginners we learn concepts in this order:

```text
1. What is JavaScript?

2. Script Tag

3. Console.log()

4. Variables

5. Data Types

6. Operators

7. Functions

8. Events

9. DOM

10. Simple Counter Example
```

---

# Section 1 – What is JavaScript?

## Ask Students

What happens when you click "Like" on Instagram?

Students:

> It likes the post.

Ask:

> Does HTML do that?

Answer:

> No.

---

What happens when Amazon updates your basket total instantly?

Students:

> It changes.

Ask:

> Is that CSS?

Answer:

> No.

---

Explain:

JavaScript allows websites to:

* React
* Calculate
* Update
* Validate
* Interact

---

## Real World Examples

### Instagram

```text
Like Button
```

JavaScript.

---

### Amazon

```text
Basket Total Updates
```

JavaScript.

---

### Netflix

```text
Movie Recommendations
```

JavaScript.

---

### Gmail

```text
Refresh Inbox Without Reload
```

JavaScript.

---

# Section 2 – JavaScript in HTML

Show students:

```html
<script>

alert("Hello COM109");

</script>
```

Explain:

```text
HTML
=
Structure

JavaScript
=
Instructions
```

---

# First JavaScript Program

```html
<button onclick="alert('Hello')">
Click Me
</button>
```

When the button is clicked:

1. User performs action
2. JavaScript runs
3. Browser responds

---

# Section 3 – Console

Before writing complex programs, developers use the Console.

Open:

```text
Right Click

↓

Inspect

↓

Console
```

---

Run:

```javascript
console.log("Hello World");
```

---

Run:

```javascript
console.log("COM109");
```

---

Run:

```javascript
console.log("JavaScript");
```

---

## Student Activity

Ask every student to print:

* Their name
* Their favourite food
* Their favourite app

using `console.log()`.

---

# Section 4 – Variables

## What is a Variable?

A variable stores information.

Think of a variable as a labelled box.

---

Draw:

```text
BOX

[Vishnu]
```

---

Example:

```javascript
let name = "Vishnu";
```

---

Explain:

```text
Variable Name
=
name

Stored Value
=
Vishnu
```

---

More Examples

```javascript
let age = 20;
```

```javascript
let city = "London";
```

```javascript
let university = "QA";
```

---

Display values:

```javascript
console.log(name);
console.log(age);
console.log(city);
```

---

## Student Activity

Create variables:

```javascript
let favouriteMovie
let favouriteFood
let favouriteSport
```

Then print them.

---

# Section 5 – Data Types

JavaScript stores different kinds of data.

---

## String

Text.

```javascript
let name = "John";
```

---

## Number

Numeric values.

```javascript
let age = 20;
```

---

## Boolean

True or False.

```javascript
let isStudent = true;
```

---

## Ask Students

What type is:

```javascript
"Netflix"
```

Answer:

String.

---

What type is:

```javascript
99
```

Answer:

Number.

---

What type is:

```javascript
false
```

Answer:

Boolean.

---

# Section 6 – Operators

Operators perform calculations.

---

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

## Modulus

```javascript
15 % 9
```

Result:

```javascript
6
```

---

## Real World Example

Amazon Basket:

```javascript
let basketTotal = 100;
let deliveryCharge = 5;

console.log(basketTotal + deliveryCharge);
```

---

## Student Activity

Calculate:

```javascript
let maths = 80;
let science = 70;

console.log(maths + science);
```

---

# Section 7 – Functions

## What is a Function?

A function is a reusable set of instructions.

---

Real World Analogy:

```text
Microwave Button

Press Button

↓

Instructions Run
```

---

Example:

```javascript
function sayHello() {

    console.log("Hello");

}
```

---

Run the function:

```javascript
sayHello();
```

---

Another Example:

```javascript
function greet() {

    console.log("Welcome COM109");

}
```

---

## Student Activity

Create:

```javascript
function introduceMe() {

    console.log("My name is _____");

}
```

Then run it.

---

# Section 8 – Events

An event is something that happens on a webpage.

Examples:

* Click
* Hover
* Key Press
* Page Load
* Resize

---

Draw:

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

Example:

```html
<button onclick="sayHello()">
Click Me
</button>
```

---

Real World Examples

| Event     | Website Example   |
| --------- | ----------------- |
| Click     | Add To Cart       |
| Hover     | Netflix Menu      |
| Key Press | Search Box        |
| Load      | Homepage Loading  |
| Resize    | Responsive Layout |

---

# Section 9 – DOM

The DOM is one of the most important JavaScript concepts.

---

## What is DOM?

DOM stands for:

```text
Document Object Model
```

---

Think of the DOM as:

> A map of the webpage.

---

Draw:

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

Real World Analogy:

```text
Website = House

DOM = Blueprint
```

---

JavaScript uses the DOM to find and modify elements.

Example:

```javascript
document.getElementById("title")
```

Meaning:

> Find the element called title.

---

# Section 10 – Simple Counter Example

This is similar to Instagram likes.

```javascript
let likes = 0;

function addLike() {

    likes++;

    console.log(likes);

}
```

---

Students immediately understand:

```text
Click

↓

JavaScript Runs

↓

Number Changes

↓

Updated Result
```

---

# Live Coding Session

## Demo 1

```html
<button onclick="alert('Hello')">
Click Me
</button>
```

---

## Demo 2

```javascript
console.log("Hello COM109");
```

---

## Demo 3

```javascript
let age = 20;

console.log(age);
```

---

## Demo 4

```javascript
let x = 10;
let y = 5;

console.log(x + y);
```

---

## Demo 5

```javascript
function greet() {

    console.log("Welcome");

}

greet();
```

---

## Demo 6

```javascript
let likes = 0;

function addLike() {

    likes++;

    console.log(likes);

}
```

---

# Seminar Preparation

Today's practical focuses on:

```text
Variables

↓

Operators

↓

Console

↓

Functions

↓

Events

↓

Debugging
```

---

# Key Concepts To Remember

If students understand these concepts, the week is a success:

1. What JavaScript is
2. Console.log()
3. Variables
4. Data Types
5. Operators
6. Functions
7. Events
8. DOM

Everything else later becomes easier:

* Arrays
* Loops
* Objects
* jQuery
* React
* Angular

---

# End of Lecture Summary

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
