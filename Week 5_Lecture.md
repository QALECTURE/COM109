# COM109 Client-Side Development

# Week 5 – JavaScript Arrays, Conditions and Loops

---

## Learning Outcomes

By the end of this session students should be able to:

- Explain what arrays are and why they are useful
- Access and modify array elements
- Use common array methods
- Create decision-making logic using if statements
- Use else and else-if conditions
- Understand switch statements
- Understand loops and repetition
- Use while, do-while and for loops
- Understand break and continue
- Combine arrays and loops together

---

# Why This Week Matters

Last week we learned:

```text
Variables
Functions
Events
DOM
```

This week we learn:

```text
Store Multiple Values

↓

Make Decisions

↓

Repeat Tasks
```

These three concepts are used in almost every application.

---

# Class Opening

Ask students:

### Question 1

Netflix has over 10,000 movies.

Would developers create:

```javascript
let movie1;
let movie2;
let movie3;
```

10,000 times?

No.

So how do they store lots of data?

Arrays.

---

### Question 2

How does Amazon decide whether you get free delivery?

It checks a condition.

Conditions are decision-making tools.

---

### Question 3

How does Instagram display hundreds of comments?

Loops.

---

# Fun Facts

### Fun Fact 1

Netflix stores thousands of movies and recommendations using data structures similar to arrays.

### Fun Fact 2

Google Search performs billions of loops every day.

### Fun Fact 3

Amazon uses conditions constantly:

- Discount eligibility
- Delivery options
- User permissions
- Payment validation

### Fun Fact 4

Every social media platform uses arrays to manage posts, comments and users.

---

# The Big Picture

```text
JavaScript

|
+-- Variables

|
+-- Arrays

|
+-- Conditions

|
+-- Loops
```

---

# Arrays

## What is an Array?

An array stores multiple values inside a single variable.

Without arrays:

```javascript
let student1 = "John";
let student2 = "Sarah";
let student3 = "Mike";
```

With arrays:

```javascript
let students = [
    "John",
    "Sarah",
    "Mike"
];
```

---

## Real World Example

Shopping Basket

```text
Milk
Bread
Eggs
Cheese
```

All items belong in one basket.

Arrays work in the same way.

---

## Array Indexes

Arrays start counting from:

```text
0
```

Example:

```javascript
let fruits = [
    "Apple",
    "Orange",
    "Banana"
];
```

```javascript
fruits[0]
```

Apple

```javascript
fruits[1]
```

Orange

```javascript
fruits[2]
```

Banana

---

## Array Length

```javascript
console.log(fruits.length);
```

Returns:

```text
3
```

---

# Array Methods

## push()

Adds an item to the end.

```javascript
fruits.push("Pear");
```

---

## pop()

Removes the last item.

```javascript
fruits.pop();
```

---

## shift()

Removes the first item.

```javascript
fruits.shift();
```

---

## unshift()

Adds an item to the beginning.

```javascript
fruits.unshift("Mango");
```

---

# Conditional Statements

## What is a Condition?

Conditions allow programs to make decisions.

---

## Real World Example

University Grade Check

```text
Mark >= 40

PASS

Else

FAIL
```

---

## if Statement

```javascript
let age = 20;

if(age >= 18){

    console.log("Adult");

}
```

---

## if else

```javascript
if(age >= 18){

    console.log("Adult");

}
else{

    console.log("Child");

}
```

---

## else if

```javascript
let mark = 75;

if(mark >= 70){

    console.log("First");

}
else if(mark >= 60){

    console.log("2:1");

}
else{

    console.log("Pass");

}
```

---

# Switch Statements

Used when checking multiple possible values.

```javascript
let day = 1;

switch(day){

    case 1:
        console.log("Monday");
        break;

    case 2:
        console.log("Tuesday");
        break;

    default:
        console.log("Unknown");

}
```

---

# Loops

## Why Do We Need Loops?

Instead of writing:

```javascript
console.log("Hello");
console.log("Hello");
console.log("Hello");
console.log("Hello");
```

We use loops.

---

# While Loop

```javascript
let i = 0;

while(i < 3){

    console.log(i);

    i++;

}
```

---

# Do While Loop

Runs at least once.

```javascript
let i = 0;

do{

    console.log(i);

    i++;

}
while(i < 3);
```

---

# For Loop

Most commonly used loop.

```javascript
for(let i = 0; i < 5; i++){

    console.log(i);

}
```

---

# Loop Components

```javascript
for(let i = 0; i < 5; i++)
```

| Part | Meaning |
|--------|--------|
| i = 0 | Starting value |
| i < 5 | Condition |
| i++ | Increment |

---

# break

Stops a loop completely.

```javascript
for(let i = 0; i < 10; i++){

    if(i == 5){

        break;

    }

    console.log(i);

}
```

---

# continue

Skips the current iteration.

```javascript
for(let i = 0; i < 10; i++){

    if(i == 5){

        continue;

    }

    console.log(i);

}
```

---

# Most Important Concept This Week

Arrays + Loops

```javascript
let fruits = [
    "Apple",
    "Orange",
    "Banana"
];

for(let i = 0; i < fruits.length; i++){

    console.log(fruits[i]);

}
```

This is one of the most common patterns in programming.

---

# End of Lecture Summary

```text
Arrays
=
Store Multiple Values

Conditions
=
Make Decisions

Loops
=
Repeat Tasks
```

These concepts form the foundation of modern software development.
