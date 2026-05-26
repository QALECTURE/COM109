# HTML Cheatsheet

HTML stands for **HyperText Markup Language**. It gives structure and meaning to webpage content.

## Basic HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
</head>
<body>
    Page content goes here.
</body>
</html>
```

## Headings

```html
<h1>Main heading</h1>
<h2>Section heading</h2>
<h3>Subsection heading</h3>
```

Use one `h1` for the main page heading. Use `h2` and lower levels for sections.

## Paragraphs

```html
<p>This is a paragraph of text.</p>
```

Paragraphs are used for normal blocks of text.

## Links

```html
<a href="https://developer.mozilla.org/">Visit MDN Web Docs</a>
```

Links use the `href` attribute to say where they go.

## Images

```html
<img src="images/profile.jpg" alt="Profile photo of a student developer">
```

The `src` attribute points to the image file. The `alt` attribute describes the image for accessibility.

## Lists

Unordered list:

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

Ordered list:

```html
<ol>
    <li>Create the file</li>
    <li>Add HTML</li>
    <li>Open in the browser</li>
</ol>
```

## Forms

```html
<form>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">

    <button type="submit">Submit</button>
</form>
```

Forms collect information from users.

## Common Input Types

```html
<input type="text">
<input type="email">
<input type="password">
<input type="number">
<input type="date">
```

## Text Area

```html
<textarea name="message" rows="5"></textarea>
```

Use `textarea` when the user needs to write a longer message.

## Semantic Tags

Semantic tags describe the purpose of content.

```html
<header>Top of the page</header>
<nav>Navigation links</nav>
<main>Main content</main>
<section>A grouped section</section>
<article>A self-contained piece of content</article>
<footer>Bottom of the page</footer>
```

Semantic HTML helps browsers, search engines, screen readers and developers understand the page.

