# COM109 Client-Side Development

# Week 6 – JavaScript Functions & Browser Storage

---

# 🎯 Learning Outcomes

By the end of today's lecture, you should be able to:

- Explain what a function is.
- Create and call JavaScript functions.
- Understand parameters and return values.
- Explain local and global variables.
- Understand why websites use Cookies.
- Explain LocalStorage and SessionStorage.
- Build reusable JavaScript code.

---

# 🚀 Class Opening (5 Minutes)

Ask students:

## Question 1

Imagine you work for Amazon.

When a customer clicks:

```
Add to Basket
```

100 times...

Should the developer write:

```javascript
basket1();
basket2();
basket3();
basket4();
```

100 different functions?

Students:

"No."

Exactly.

Developers write ONE function.

That function can run hundreds or thousands of times.

That is today's topic.

---

## Question 2

When you reopen Spotify...

How does it remember:

- Dark Mode
- Volume
- Language
- Last Played Song

Students usually answer:

"It saves it somewhere."

Exactly.

Today we'll learn **where** it saves it.

---

# 💡 Tech Facts

### Fun Fact #1

Google Chrome executes millions of JavaScript functions every second across all open tabs.

---

### Fun Fact #2

React (used by Facebook, Instagram and Netflix) is built almost entirely using JavaScript functions.

---

### Fun Fact #3

Every time you press "Like" on Instagram...

A JavaScript function runs.

---

### Fun Fact #4

Netflix remembers exactly where you stopped watching using browser storage.

---

# 🏗 Big Picture

Draw this.

```text
Website

↓

HTML

Structure

↓

CSS

Looks Beautiful

↓

JavaScript

Behaviour

↓

Functions

Reusable Code

↓

Browser Storage

Remember Users
```

Tell students:

Last week we learned:

```
Arrays

Conditions

Loops
```

Today we learn:

```
Write Once

Use Forever
```

---

# 📌 What Is A Function?

Simple explanation:

A function is a reusable block of code.

Instead of writing the same instructions again and again...

We write them once.

---

# ☕ Real World Analogy

Coffee Machine

```
Press Button

↓

Machine Makes Coffee
```

Every time you press...

The same instructions run.

Functions work exactly the same way.

---

# Interactive Question

Ask:

Why don't coffee machines need a new program every time someone wants coffee?

Students:

Because the instructions already exist.

Exactly.

Functions are reusable instructions.

---

# Function Declaration

General structure:

```javascript
function sayHello(){

}
```

Explain each part.

```
function

↓

Tells JavaScript we are creating a function

↓

sayHello

↓

Function Name

↓

()

↓

Parameters

↓

{}

↓

Instructions
```

---

# Live Demo

```javascript
function sayHello(){

    console.log("Hello COM109");

}
```

Ask students:

Will this print anything?

Students:

Maybe.

Run it.

Nothing happens.

---

Explain:

Creating a function DOES NOT execute it.

---

# Function Calling

Now show:

```javascript
sayHello();
```

Output:

```
Hello COM109
```

---

Ask:

What changed?

Students:

We called the function.

Exactly.

---

Call it again.

```javascript
sayHello();
sayHello();
sayHello();
```

Students immediately understand:

Write once.

Reuse forever.

---

# Real World Example

Imagine Netflix.

Instead of creating

```
playMovie1()

playMovie2()

playMovie3()
```

They use:

```javascript
playMovie();
```

Again and again.

---

# Local Variables

Ask:

Can everyone access your bedroom?

No.

Only you.

---

Draw:

```
House

↓

Bedroom

↓

Private
```

Now explain:

Variables created inside a function are private.

Example:

```javascript
function student(){

    let name = "John";

    console.log(name);

}
```

Outside:

```javascript
console.log(name);
```

Produces an error.

---

Question:

Why?

Because the variable only exists inside the function.

---

# Outer (Global) Variables

Now explain.

Outside:

```javascript
let university = "QA";
```

Function:

```javascript
function welcome(){

    console.log(university);

}
```

Works perfectly.

Explain:

Functions can access variables created outside them.

---

Real World Example

Imagine:

```
Classroom

↓

Projector

Everyone can use it.
```

Global.

```
Student Notebook

↓

Only that student.
```

Local.

---

# Parameters

Ask:

Can one coffee machine make:

- Small
- Medium
- Large

Yes.

How?

It receives instructions.

Functions work the same way.

---

Example:

```javascript
function greet(name){

    console.log("Hello " + name);

}
```

Now call:

```javascript
greet("John");
greet("Sarah");
greet("Mike");
```

Explain:

The function stays the same.

Only the input changes.

---

Student Activity

Create:

```javascript
function welcome(student){

    console.log("Welcome " + student);

}
```

Try it with your own name.

---

# Default Parameters

Question:

What if someone forgets to enter their name?

Instead of showing:

```
Hello undefined
```

We provide a default.

```javascript
function greet(name="Guest"){

    console.log(name);

}
```

Call:

```javascript
greet();
```

Output:

```
Guest
```

---

# Return Values

Ask:

What does a calculator do?

Students:

Returns an answer.

Exactly.

Functions can return answers too.

---

Example

```javascript
function add(a,b){

    return a+b;

}
```

Now:

```javascript
let answer = add(5,3);

console.log(answer);
```

Output

```
8
```

Explain:

```
Input

↓

Process

↓

Return Result
```

---

# Good Function Names

Show:

```
calculateTotal()

showMessage()

checkAge()

createAccount()

getUser()
```

Explain:

Good names explain exactly what the function does.

---

Bad example:

```
abc()

test()

hello()

x()
```

Students should avoid these.

---

# One Function = One Job

Ask:

Should one function:

```
Login User

↓

Print Receipt

↓

Play Music

↓

Send Email
```

Students laugh.

Answer:

No.

One function should perform ONE task.

---

# Function Expressions

Simple explanation.

Instead of:

```javascript
function greet(){

}
```

We can also write:

```javascript
let greet = function(){

};
```

Both create functions.

---

# Callback Functions

Keep this simple.

Don't go deep.

Ask:

Imagine ordering food.

You place an order.

Do you get it immediately?

No.

Restaurant prepares it first.

Later...

It arrives.

That is similar to a callback.

JavaScript says:

```
Do this later.
```

Example:

```javascript
button.onclick = function(){

    alert("Clicked");

};
```

---

# Browser Storage

Ask:

How does Netflix remember:

```
Continue Watching
```

Students:

Storage.

Exactly.

---

# Cookies

Cookies are tiny pieces of information stored by the browser.

Usually used for:

- Login
- Authentication
- Remember Me

Diagram:

```
Login

↓

Server

↓

Cookie Created

↓

Browser Stores Cookie

↓

Next Visit

↓

Already Logged In
```

---

# LocalStorage

Think:

```
Permanent Notebook
```

Stored until deleted.

Example uses:

- Dark Mode
- Language
- Username
- Shopping Basket

---

# SessionStorage

Think:

```
Whiteboard

↓

Erase when class ends
```

Stored only while the browser tab is open.

---

# Comparison

| Feature | Cookies | LocalStorage | SessionStorage |
|----------|----------|--------------|----------------|
| Login | ✅ | ❌ | ❌ |
| Dark Mode | ❌ | ✅ | ❌ |
| Basket | ✅ | ✅ | ❌ |
| Temporary Form | ❌ | ❌ | ✅ |

---

# Class Discussion

Ask:

Where would you store:

✅ Dark Mode

Students:

LocalStorage

---

Login Token

Students:

Cookie

---

Temporary Quiz Answers

Students:

SessionStorage

---

# Today's Key Takeaways

```
Functions

↓

Reusable Code

↓

Parameters

↓

Input

↓

Return

↓

Output

↓

Cookies

↓

Remember Login

↓

LocalStorage

↓

Remember User Preferences

↓

SessionStorage

↓

Temporary Storage
```

---

# Before the Lab

Ask these questions.

1. Why do developers use functions?

Answer:

To avoid repeating code.

---

2. What is the difference between local and global variables?

Answer:

Local variables only exist inside the function.

Global variables can be accessed anywhere.

---

3. What is a parameter?

Answer:

Information passed into a function.

---

4. What does return do?

Answer:

Sends a result back.

---

5. Which storage remembers dark mode?

Answer:

LocalStorage.

---

6. Which storage is usually used for login?

Answer:

Cookies.

---

7. Which storage disappears after closing the browser tab?

Answer:

SessionStorage.
