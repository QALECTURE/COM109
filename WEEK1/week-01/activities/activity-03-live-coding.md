# Activity 03: Live Coding `index.html`

## Purpose

Guide students through creating a first HTML page while hearing the lecturer explain each decision.

## Time

25 to 35 minutes

## Setup

Open VS Code with an empty folder called `my-first-portfolio`. Create a file named `index.html`.

## Part 1: HTML Boilerplate

**What to say:**  
"Every HTML page needs a basic structure. This tells the browser what type of document it is, what language it uses and where the page content begins."

**What to type:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Portfolio</title>
</head>
<body>

</body>
</html>
```

**What students should see:**  
A blank page in the browser with the tab title "My First Portfolio".

## Part 2: Header

**What to say:**  
"The header is the introduction to the page. It usually contains the name, title or main branding."

**What to type:**

```html
<header>
    <h1>Your Name</h1>
    <p>Beginner web developer and COM109 student</p>
</header>
```

**What students should see:**  
A large heading and a short line of text.

## Part 3: Navigation

**What to say:**  
"Navigation helps people move around the page. These links will jump to sections using IDs."

**What to type:**

```html
<nav>
    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
```

**What students should see:**  
A small list of links. They may not jump yet until the matching sections exist.

## Part 4: Main and About Section

**What to say:**  
"The main element contains the main content of the page. Sections help us group related content."

**What to type:**

```html
<main>
    <section id="about">
        <h2>About Me</h2>
        <p>I am learning how websites are built using HTML, CSS and JavaScript.</p>
    </section>
</main>
```

**What students should see:**  
An "About Me" section appears under the navigation.

## Part 5: Skills List

**What to say:**  
"Lists are useful when we have several related items. Skills, ingredients, steps and menu links often use lists."

**What to type:**

```html
<section id="skills">
    <h2>Skills</h2>
    <ul>
        <li>HTML basics</li>
        <li>Using VS Code</li>
        <li>Browser DevTools</li>
        <li>GitHub basics</li>
    </ul>
</section>
```

**What students should see:**  
A bullet-point list of skills.

## Part 6: Contact Form

**What to say:**  
"Forms are how users send information. Login pages, search bars, checkout pages and booking forms all use form concepts."

**What to type:**

```html
<section id="contact">
    <h2>Contact Me</h2>
    <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name">

        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <button type="submit">Send</button>
    </form>
</section>
```

**What students should see:**  
Two input boxes and a button.

## Part 7: Footer

**What to say:**  
"The footer normally contains closing information such as copyright, contact links or extra navigation."

**What to type:**

```html
<footer>
    <p>&copy; 2026 Your Name. Built for COM109.</p>
</footer>
```

**What students should see:**  
A short footer at the bottom of the page.

## Wrap-Up

Ask students:

- What does HTML control?
- Which tag felt most useful?
- What would CSS improve on this page?
- What would JavaScript add later?

