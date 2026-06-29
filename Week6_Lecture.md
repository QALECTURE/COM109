# COM109 Client-Side Development

# Week 6 – JavaScript Loops

> **Theme of this Week**
>
> Last week we learned how JavaScript stores information using arrays and makes decisions using conditions.
>
> This week we answer a new question:
>
> **"How can a computer perform the same task hundreds or even millions of times without us writing the same code repeatedly?"**
>
> The answer is **Loops**.

---

# Learning Outcomes

By the end of this session, you should be able to:

- Explain what loops are and why they are important.
- Understand the difference between `while`, `do...while` and `for` loops.
- Predict the output of loop-based programs.
- Write simple loops.
- Understand infinite loops and how to avoid them.
- Use `break` and `continue`.
- Solve real-world programming problems using loops.

---

# Before We Begin...

Let's think about something.

Imagine you work for **Netflix**.

Netflix has over **18,000 movies and TV shows**.

How would you display them?

Would a programmer write:

```javascript
console.log("Movie 1");
console.log("Movie 2");
console.log("Movie 3");
...
console.log("Movie 18000");
```

Of course not!

Instead, computers repeat the same instructions automatically.

That is exactly what loops do.

---

# Technical Fun Facts

## Fun Fact #1

Google processes **billions of searches every day**.

Every search involves loops behind the scenes.

---

## Fun Fact #2

Instagram may display hundreds of comments on one post.

JavaScript loops help display them efficiently.

---

## Fun Fact #3

Spotify uses loops to build playlists.

Each song is processed one after another.

---

## Fun Fact #4

Amazon loops through products whenever you search for something.

Imagine searching for:

> Wireless Mouse

Amazon checks thousands of products almost instantly.

---

# Real World Analogy

Imagine a teacher taking attendance.

Without loops:

```text
John?

Sarah?

Mike?

Emma?

David?

...
```

Imagine there are **300 students**.

That would be exhausting.

Instead, the teacher repeats the same question until everyone has been called.

That is exactly how a loop works.

---

# Big Picture

Draw this on the board.

```text
JavaScript

↓

Variables

↓

Conditions

↓

Loops

↓

Automation
```

Explain:

Variables store information.

Conditions make decisions.

Loops automate repetitive work.

---

# What Is A Loop?

A loop repeats a block of code while a condition is true.

Think of it like:

```text
Start

↓

Check Condition

↓

Do Work

↓

Go Back

↓

Check Again

↓

Repeat
```

---

# Where Are Loops Used?

Students use these applications every day.

| Application | Loop Used For |
|-------------|--------------|
| Netflix | Display movies |
| Amazon | Display products |
| Spotify | Play playlists |
| Instagram | Display comments |
| Google Search | Process results |
| Facebook | Load posts |
| YouTube | Show recommended videos |

Ask students:

> Can you think of another application that repeats tasks?

---

# Why Do We Need Loops?

Without loops:

```javascript
console.log("Hello");
console.log("Hello");
console.log("Hello");
console.log("Hello");
console.log("Hello");
```

Now imagine printing:

```text
Hello
```

10,000 times.

Impossible to write manually.

Instead:

```javascript
for(let i = 0; i < 5; i++){

    console.log("Hello");

}
```

---

# Interactive Question

Ask:

> If I wanted to print "QA" 1000 times...

Would I write:

```javascript
console.log("QA");
```

1000 times?

Students should answer:

> No.

Exactly.

---

# Understanding Loop Components

Every loop has three parts.

```text
Start

↓

Condition

↓

Update
```

Draw:

```text
Start

↓

Check

↓

Run Code

↓

Increase Counter

↓

Repeat
```

---

# While Loop

The simplest loop.

Syntax:

```javascript
while(condition){

    // code

}
```

---

## Example

```javascript
let i = 1;

while(i <= 5){

    console.log(i);

    i++;

}
```

---

# Walk Through Slowly

Initial value:

```text
i = 1
```

Question:

Is

```text
1 <= 5
```

True?

Yes.

Print:

```text
1
```

Increase.

```text
i = 2
```

Repeat.

Continue until:

```text
i = 6
```

Now:

```text
6 <= 5
```

False.

Loop stops.

---

# Flow Diagram

```text
Start

↓

i = 1

↓

Condition

↓

True?

↓

Print

↓

Increase i

↓

Back to Condition

↓

False?

↓

Stop
```

---

# Real World Example

Imagine a security guard checking IDs.

```text
Student arrives

↓

Check ID

↓

Valid?

↓

Allow Entry

↓

Next Student

↓

Repeat
```

---

# Common Beginner Mistake

```javascript
let i = 1;

while(i <= 5){

    console.log(i);

}
```

Question:

What is missing?

Students:

```text
i++
```

Exactly.

Without it, the loop never ends.

---

# Infinite Loops

Explain:

An infinite loop never stops.

Example:

```javascript
while(true){

    console.log("Hello");

}
```

Never write loops like this unless you intentionally want them.

---

# Do...While Loop

Unlike the while loop...

A do...while loop always runs **at least once**.

Syntax:

```javascript
do{

    // code

}
while(condition);
```

---

## Example

```javascript
let number = 1;

do{

    console.log(number);

    number++;

}
while(number <= 5);
```

---

# Real World Example

ATM Machine

```text
Insert Card

↓

Show Menu

↓

Check Choice

↓

Continue?

↓

Repeat
```

The menu appears **before** checking whether the customer wants another transaction.

---

# While vs Do...While

| while | do...while |
|---------|------------|
| Checks condition first | Runs first |
| May never execute | Always executes once |

Ask students:

Which one would an ATM use?

Answer:

do...while

---

# The For Loop

This is the loop used most often in JavaScript.

Syntax:

```javascript
for(let i = 0; i < 5; i++){

    console.log(i);

}
```

---

# Breaking It Down

```javascript
let i = 0;
```

Starting point.

---

```javascript
i < 5
```

Condition.

---

```javascript
i++
```

Increase the counter.

---

# Flow Diagram

```text
Start

↓

Initialise

↓

Condition

↓

Run Code

↓

Increment

↓

Repeat
```

---

# Interactive Activity

Ask students:

How many numbers will be printed?

```javascript
for(let i = 0; i < 3; i++){

    console.log(i);

}
```

Answer:

```text
0

1

2
```

Three values.

---

# Even Numbers Example

```javascript
for(let i = 2; i <= 10; i += 2){

    console.log(i);

}
```

Output:

```text
2

4

6

8

10
```

Ask students:

Why are we increasing by **2** instead of **1**?

---

# Looping Through Arrays

This is one of the most common programming patterns.

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

Explain:

The loop visits each item inside the array.

---

# Real World Example

Spotify Playlist

```text
Song 1

↓

Song 2

↓

Song 3

↓

Song 4

↓

Finished
```

Exactly the same idea.

---

# break Statement

Sometimes we want to stop early.

Example:

```javascript
for(let i = 0; i < 10; i++){

    if(i == 5){

        break;

    }

    console.log(i);

}
```

Output:

```text
0

1

2

3

4
```

Loop stops at 5.

---

# continue Statement

Instead of stopping...

Skip only one iteration.

```javascript
for(let i = 0; i < 6; i++){

    if(i == 3){

        continue;

    }

    console.log(i);

}
```

Output:

```text
0

1

2

4

5
```

3 is skipped.

---

# Real World Example

Teacher Taking Attendance

```text
Student Absent

↓

Skip

↓

Next Student
```

That is exactly how continue works.

---

# Live Coding Session

## Demo 1

Print numbers 1–5 using while.

---

## Demo 2

Print your name five times.

---

## Demo 3

Use a do...while loop.

---

## Demo 4

Create a simple for loop.

---

## Demo 5

Print even numbers.

---

## Demo 6

Loop through an array of student names.

---

## Demo 7

Use break.

---

## Demo 8

Use continue.

---

# Common Beginner Mistakes

❌ Forgetting to increase the counter.

❌ Creating an infinite loop.

❌ Starting arrays at index 1 instead of 0.

❌ Forgetting the loop condition.

❌ Confusing `<` with `<=`.

---

# Career Connection

Every software developer uses loops.

Examples:

- Frontend Developer
- Backend Developer
- Game Developer
- AI Engineer
- Data Scientist
- Mobile App Developer
- Cyber Security Engineer

Whenever software needs to process many pieces of information...

Loops are used.

---

# Reflection Questions

Discuss these with the class.

1. Why are loops better than writing the same code repeatedly?
2. What is the difference between `while` and `for`?
3. When would you use a `do...while` loop?
4. Why is an infinite loop dangerous?
5. Where have you used loops today without realising it?

---

# End of Lecture Summary

```text
Variables
↓

Store Data

Conditions
↓

Make Decisions

Loops
↓

Repeat Tasks

Arrays + Loops
↓

Process Multiple Items Automatically
```

## Key Takeaways

✅ Loops automate repetitive tasks.

✅ `while` checks the condition first.

✅ `do...while` runs at least once.

✅ `for` is the most commonly used loop.

✅ `break` stops a loop.

✅ `continue` skips one iteration.

✅ Loops are used in almost every modern application, from Netflix and Amazon to Google and Spotify.

---

# Preview of Next Week

Next week we will combine everything we have learned:

- Variables
- Arrays
- Conditions
- Loops
- Functions
- DOM Manipulation

to build more interactive web applications where JavaScript responds to user actions in real time.
