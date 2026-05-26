# Lab: Build Your First Developer Portfolio Website

## Objective

Create a simple HTML-only developer portfolio webpage. By the end of the lab, you will have a page that introduces you, lists your skills, links to useful websites and includes a basic contact form.

## Tools Needed

- VS Code
- A web browser such as Chrome, Edge, Firefox or Safari
- GitHub account

## Expected Output

Your final page should include:

- A main heading with your name
- A short introduction
- An about section
- A list of skills
- A projects section
- An image
- Useful links
- A contact form
- A footer

## Step 1: Create a Project Folder

1. Create a folder called `my-first-portfolio`.
2. Open the folder in VS Code.
3. Inside the folder, create a file called `index.html`.

## Step 2: Add the HTML Boilerplate

Add the basic structure of an HTML page:

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

Open the file in your browser. The page will look blank for now, and that is normal.

## Step 3: Add a Heading

Inside the `body`, add:

```html
<h1>Your Name</h1>
<p>Beginner web developer and COM109 student.</p>
```

Replace `Your Name` with your own name.

## Step 4: Add an About Section

Use a `section` element:

```html
<section>
    <h2>About Me</h2>
    <p>I am learning how websites are built using HTML, CSS and JavaScript.</p>
</section>
```

Keep it short and realistic. You can mention your course, interests or career goals.

## Step 5: Add a Skills List

Add a list of skills you are starting to learn:

```html
<section>
    <h2>Skills</h2>
    <ul>
        <li>HTML basics</li>
        <li>Using VS Code</li>
        <li>Browser DevTools</li>
        <li>GitHub basics</li>
    </ul>
</section>
```

## Step 6: Add an Image

Add an image using the `img` tag:

```html
<img src="images/profile-placeholder.jpg" alt="Profile placeholder image">
```

If you do not have an image yet, you can use a placeholder image or add a note to include one later. The `alt` text is important for accessibility.

## Step 7: Add Useful Links

Add links to websites that help you learn:

```html
<section>
    <h2>Useful Links</h2>
    <ul>
        <li><a href="https://developer.mozilla.org/">MDN Web Docs</a></li>
        <li><a href="https://www.freecodecamp.org/">freeCodeCamp</a></li>
        <li><a href="https://github.com/">GitHub</a></li>
    </ul>
</section>
```

## Step 8: Add a Contact Form

Forms allow users to enter information:

```html
<section>
    <h2>Contact Me</h2>
    <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name">

        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <label for="message">Message:</label>
        <textarea id="message" name="message"></textarea>

        <button type="submit">Send Message</button>
    </form>
</section>
```

This form will not send data yet. Later in the module, you will learn how JavaScript can improve form behaviour.

## Step 9: Add Semantic Structure

Improve your page by using:

- `header` for the top of the page
- `nav` for navigation links
- `main` for the main content
- `section` for grouped content
- `footer` for the bottom of the page

## Step 10: Save and Test

1. Save your file.
2. Refresh the browser.
3. Check that headings, links, lists and the form appear correctly.
4. Right-click the page and choose **Inspect** to view the HTML in DevTools.

## Final Challenge

Add a `Projects` section with two project ideas you would like to build during this module. Examples:

- A personal portfolio
- A cinema booking page
- A recipe website
- A student budgeting tool
- A small interactive quiz

## Stretch Challenge

Try adding:

- A navigation menu that links to sections on the same page
- A table showing your weekly learning goals
- A second image
- Links that open in a new tab using `target="_blank"`

## Student Reflection Questions

Answer these at the end of the lab:

- What part of HTML felt easiest today?
- What part felt confusing?
- Why is it useful to structure content before styling it?
- Where do you see forms in real websites such as Amazon, Uber, Monzo or university systems?
- What would you like your portfolio to include by the end of the module?

