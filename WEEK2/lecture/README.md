# COM109 Week 2 Lecture – CSS and Web Accessibility

## Lecturer Overview

This lecture introduces CSS as the language that controls presentation, layout and visual polish on the web. It also introduces accessibility as a professional responsibility, not an optional extra. The goal is for students to understand how CSS connects to HTML, how common selectors work, why external stylesheets matter, and how design choices affect real users.

By the end of the session, students should be able to:

- Explain the role of CSS in a web page.
- Write basic CSS selectors and declarations.
- Compare inline, internal and external CSS.
- Use classes and IDs appropriately.
- Describe the cascade, specificity and the box model.
- Recognise block, inline and inline-block behaviour.
- Explain why responsive design, print CSS and accessibility matter.
- Validate CSS using the W3C CSS Validator.

Suggested timing for a 2-hour session:

- 10 minutes: opening hook and Week 1 recap
- 20 minutes: HTML, CSS, JavaScript and CSS syntax
- 25 minutes: selectors, classes, IDs, cascade and specificity
- 20 minutes: colours, fonts and the box model
- 15 minutes: block, inline and responsive design
- 20 minutes: accessibility, WCAG, POUR and validation
- 10 minutes: live demo setup and questions

## 1. Opening Hook / Fun Facts

Simple explanation:
CSS is what makes websites look designed instead of looking like plain documents. HTML gives the page meaning and structure; CSS gives it layout, colour, spacing and visual identity.

Real-world analogy:
HTML is the building structure. CSS is the interior design, paint, lighting, signs and furniture layout.

Real tech example:
Apple, Netflix, Monzo, Revolut and TikTok all rely on CSS to create interfaces that feel polished and deliberate. Without CSS, Apple.com would look like a plain document with headings, paragraphs and links.

What to say to students:
"Today we move from writing page content to controlling how that content feels. Good CSS is one reason apps feel expensive, professional and easy to trust."

Quick student question:
"Think of a website or app that feels premium. What visual choices make it feel that way?"

Fun facts to mention:

- CSS is what makes websites look premium.
- Without CSS, Apple.com would look like a plain document.
- Accessibility helps disabled users but also improves usability for everyone.
- Good CSS is one reason apps feel expensive and professional.
- GOV.UK is a strong example of simple, accessible design.

## 2. Recap From Week 1

Simple explanation:
In Week 1, students focused on HTML: headings, paragraphs, links, images, lists and page structure. HTML tells the browser what each piece of content is.

Real-world analogy:
If a menu says "Coffee", "Tea" and "Cake", HTML labels those items. CSS decides whether the menu appears as a plain list, a modern cafe card or a mobile-friendly layout.

Real tech example:
BBC News articles use HTML to identify headings, article text, images, captions and navigation. CSS then controls column widths, font sizes, colours and spacing.

What to say to students:
"Last week, we created meaning. This week, we create presentation while keeping that meaning clear."

Quick student question:
"Why is it useful for a browser to know that something is a heading rather than just large bold text?"

## 3. What CSS Is

Simple explanation:
CSS stands for Cascading Style Sheets. It is used to style HTML elements. CSS can change colours, fonts, spacing, borders, layout and how a page adapts to different screen sizes.

Real-world analogy:
HTML is a recipe list. CSS is how the finished meal is plated and presented.

Real tech example:
Amazon product pages use CSS to make product images large, prices noticeable, buttons clear and delivery information easy to scan.

What to say to students:
"CSS does not usually change what the content means. It changes how that content is presented."

Quick student question:
"What would happen to an online shop if every button, price and heading looked the same?"

## 4. Why CSS Matters In Industry

Simple explanation:
CSS affects usability, branding, accessibility, customer trust and conversion. In real teams, front-end developers use CSS to turn designs into working interfaces.

Real-world analogy:
A restaurant with confusing signs and cramped tables may serve good food, but customers still struggle. A website can have good content and still fail if the interface is hard to use.

Real tech example:
Monzo and Revolut use clean spacing, strong hierarchy and consistent components so users can understand financial information quickly.

What to say to students:
"CSS is not decoration only. It helps users make decisions, avoid mistakes and trust what they are seeing."

Quick student question:
"Why might banks and health services care about simple, readable design?"

## 5. HTML vs CSS vs JavaScript

Simple explanation:
HTML provides structure and meaning. CSS controls presentation and layout. JavaScript adds behaviour and interaction.

Real-world analogy:
For a car, HTML is the frame and seats, CSS is the paint and dashboard layout, and JavaScript is the engine control and interactive features.

Real tech example:
On Netflix, HTML structures titles and descriptions, CSS styles rows and cards, and JavaScript handles interactions such as carousel movement and video playback controls.

What to say to students:
"A complete front-end experience usually needs all three languages, but each one has a different job."

Quick student question:
"On TikTok, which part is likely responsible for the play button doing something when clicked?"

Diagram:

```text
Web page
├── HTML        = structure and meaning
├── CSS         = style, layout and presentation
└── JavaScript  = behaviour and interaction
```

## 6. CSS Syntax Explained Simply

Simple explanation:
A CSS rule has a selector and a declaration block. The selector chooses the HTML element. The declarations describe the styles to apply.

Real-world analogy:
"All staff must wear black shoes" is like a CSS rule. "All staff" is the selector. "Wear black shoes" is the declaration.

Real tech example:
GOV.UK uses consistent styles for headings, links, buttons and form fields across many services.

What to say to students:
"Read CSS as instructions: find this thing, then apply these visual rules."

Quick student question:
"In `p { color: blue; }`, which part selects the element?"

Example:

```css
p {
  color: blue;
  font-size: 18px;
}
```

## 7. CSS Selectors

### Element Selector

Simple explanation:
An element selector targets every matching HTML element.

Real-world analogy:
"All chairs in this room should face forward."

Real tech example:
BBC might style all paragraph text consistently across an article.

What to say to students:
"Use element selectors when you want a general rule for every element of that type."

Quick student question:
"What happens if we write `h2 { color: green; }`?"

```css
h2 {
  color: green;
}
```

### Class Selector

Simple explanation:
A class selector targets any element with a matching class attribute. Classes are reusable.

Real-world analogy:
Several people can wear a "team leader" badge. The badge describes a role, not one unique person.

Real tech example:
Amazon can reuse button classes for "Add to Basket" and other call-to-action buttons.

What to say to students:
"Classes are the everyday tool for reusable styling."

Quick student question:
"Why is a class useful when several menu items need the same style?"

```html
<p class="highlight">Popular choice</p>
```

```css
.highlight {
  background-color: yellow;
}
```

### ID Selector

Simple explanation:
An ID selector targets one unique element on a page.

Real-world analogy:
A student ID number belongs to one student only.

Real tech example:
A page might use `id="main-content"` so a skip link can jump straight to the main content.

What to say to students:
"Use IDs when something is unique. For repeated styling, prefer classes."

Quick student question:
"Should every menu row have the same ID? Why not?"

```html
<main id="main-content">
```

```css
#main-content {
  max-width: 800px;
}
```

Diagram:

```text
CSS selector targeting

p              -> targets every <p>
.menu-item     -> targets elements with class="menu-item"
#main-content  -> targets the one element with id="main-content"
```

## 8. Inline CSS, Internal CSS, External CSS

Simple explanation:
Inline CSS is written inside an HTML element. Internal CSS is written inside a `<style>` element in the HTML file. External CSS is written in a separate `.css` file and linked from HTML.

Real-world analogy:
Inline CSS is like writing an instruction on one chair. Internal CSS is like writing rules on the classroom wall. External CSS is like having a professional style guide that many rooms can share.

Real tech example:
Large organisations such as NHS, GOV.UK and Apple need external stylesheets so thousands of pages can share consistent design.

What to say to students:
"We learn all three so you can recognise them, but real projects usually prefer external CSS."

Quick student question:
"Which approach would be easiest to update across 100 pages?"

```html
<!-- Inline -->
<p style="color: red;">Important</p>

<!-- Internal -->
<style>
  p { color: red; }
</style>

<!-- External -->
<link rel="stylesheet" href="style.css">
```

## 9. Why External CSS Is Preferred In Real Projects

Simple explanation:
External CSS keeps structure and styling separate. It is easier to maintain, reuse and cache.

Real-world analogy:
A restaurant chain uses one brand guide rather than redesigning each menu from scratch.

Real tech example:
Deliveroo can keep buttons, cards and typography consistent across many pages and screens.

What to say to students:
"External CSS is cleaner because HTML stays focused on content and CSS stays focused on presentation."

Quick student question:
"If a company changes its brand colour, where would you rather update it: one CSS file or every HTML page?"

Diagram:

```text
Browser loading HTML and CSS

index.html
   |
   | contains <link rel="stylesheet" href="style.css">
   v
style.css
   |
   v
Browser combines structure + style and displays the page
```

## 10. Cascade And Specificity

Simple explanation:
The cascade decides which CSS rule wins when more than one rule targets the same element. Specificity is the browser's way of deciding which selector is more precise.

Real-world analogy:
A general school rule might say "wear uniform", but a specific PE rule might say "wear trainers for PE". The more specific situation wins.

Real tech example:
An NHS service may have general link styles but special button styles for important actions.

What to say to students:
"When CSS surprises you, ask: which rule is more specific, and which rule appears later?"

Quick student question:
"Which feels more specific: styling every paragraph, or styling one paragraph with a class?"

Diagram:

```text
Cascade priority, simplified

Inline style            highest priority
ID selector             very specific
Class selector          reusable and common
Element selector        broad
Browser default styles  lowest priority

If priority is equal, the later rule usually wins.
```

## 11. Colours

Simple explanation:
CSS can describe colours using names, HEX values and RGB values.

Real-world analogy:
Colour names are like saying "blue". HEX and RGB are like giving an exact paint code.

Real tech example:
Monzo's bright coral and GOV.UK's strong blue are deliberate brand colours, not random choices.

What to say to students:
"Colour is not just taste. It affects readability, brand recognition and accessibility."

Quick student question:
"Why might pale grey text on a white background be a problem?"

```css
h1 {
  color: navy;           /* colour name */
  color: #005ea5;        /* HEX */
  color: rgb(0, 94, 165); /* RGB */
}
```

## 12. Fonts And Fallback Fonts

Simple explanation:
The `font-family` property controls the typeface. Fallback fonts are backup choices if the first font is unavailable.

Real-world analogy:
If your first-choice lecturer is unavailable, a backup lecturer covers the class. The page still works.

Real tech example:
Apple uses carefully chosen fonts to make interfaces feel refined and consistent.

What to say to students:
"Always include fallback fonts so the page still looks acceptable on different systems."

Quick student question:
"Why might two students see slightly different fonts on different laptops?"

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}
```

## 13. Box Model

Simple explanation:
Every HTML element is treated like a box. The box has content, padding, border and margin.

Real-world analogy:
A framed picture has the image itself, space around it, a frame, and space between the frame and other objects.

Real tech example:
Amazon product cards use spacing and borders so products are easy to scan.

What to say to students:
"If your layout looks cramped or too spread out, the box model is usually involved."

Quick student question:
"Which property creates space inside the border: margin or padding?"

Diagram:

```text
Box model

+-----------------------------+
| margin                      |
|  +-----------------------+  |
|  | border                |  |
|  |  +-----------------+  |  |
|  |  | padding         |  |  |
|  |  |  +-----------+  |  |  |
|  |  |  | content   |  |  |  |
|  |  |  +-----------+  |  |  |
|  |  +-----------------+  |  |
|  +-----------------------+  |
+-----------------------------+
```

## 14. Block, Inline And Inline-Block

Simple explanation:
Block elements usually start on a new line and take full available width. Inline elements sit within text. Inline-block elements sit inline but can have width and height.

Real-world analogy:
A block element is like a full row of seats. An inline element is like one word in a sentence. Inline-block is like a small badge placed in a sentence but with its own size.

Real tech example:
Navigation links on BBC or GOV.UK often appear inline or inline-block so they can sit beside each other.

What to say to students:
"Display type affects how elements naturally sit on the page before you add advanced layout."

Quick student question:
"Would a paragraph usually be block or inline?"

```css
a {
  display: inline-block;
  padding: 8px 12px;
}
```

## 15. Responsive Design

Simple explanation:
Responsive design means a website adapts to different screen sizes, such as mobile, tablet and desktop.

Real-world analogy:
A good cafe can seat one person, a small group or a large group by rearranging the space.

Real tech example:
TikTok, NHS and Deliveroo must work well on phones because many users visit on mobile first.

What to say to students:
"We do not design for only one screen size. Real users bring real devices."

Quick student question:
"What problems appear if a desktop layout is forced onto a phone?"

Diagram:

```text
Responsive design

Desktop: [ navigation ][ main content ][ side content ]
Tablet:  [ navigation ][ main content              ]
Mobile:  [ nav ]
         [ main content ]
         [ side content ]
```

## 16. Media Queries

Simple explanation:
Media queries apply CSS only when certain conditions are true, such as the screen being below a certain width.

Real-world analogy:
Wear a coat if it is cold. Use a compact layout if the screen is narrow.

Real tech example:
Deliveroo may show a multi-column restaurant grid on desktop and a single-column list on mobile.

What to say to students:
"Media queries let CSS respond to the device."

Quick student question:
"What should happen to a three-column layout on a small phone screen?"

```css
@media (max-width: 600px) {
  .menu-card {
    padding: 16px;
  }
}
```

## 17. Print CSS

Simple explanation:
Print CSS changes how a page looks when printed. It can remove backgrounds, hide navigation and make text more readable on paper.

Real-world analogy:
A cinema poster and a printed receipt need different layouts even if they share information.

Real tech example:
NHS appointment pages, GOV.UK guidance and booking confirmations often need print-friendly layouts.

What to say to students:
"Print CSS reminds us that the web is not only viewed on screens."

Quick student question:
"What parts of a website would you hide when printing a receipt or menu?"

```html
<link rel="stylesheet" href="print.css" media="print">
```

## 18. Web Accessibility

Simple explanation:
Web accessibility means designing and building websites that disabled people can use. It also improves usability for everyone.

Real-world analogy:
A ramp helps wheelchair users, but it also helps people with prams, suitcases and deliveries.

Real tech example:
GOV.UK is designed with plain language, strong contrast, keyboard support and clear forms because public services must work for many people.

What to say to students:
"Accessibility is part of professional web development. It is about access, dignity and quality."

Quick student question:
"Who benefits from captions on a video besides deaf users?"

Diagram:

```text
Accessibility thinking workflow

Can users perceive it?
Can users operate it?
Can users understand it?
Is it robust across tools and devices?
```

## 19. WCAG And POUR Principles

Simple explanation:
WCAG stands for Web Content Accessibility Guidelines. POUR is a simple way to remember the main principles: Perceivable, Operable, Understandable and Robust.

Real-world analogy:
A public building should be visible, reachable, understandable and built to standards.

Real tech example:
NHS and GOV.UK services use accessibility standards because users may depend on them for essential tasks.

What to say to students:
"POUR gives us a practical checklist for thinking about access."

Quick student question:
"Which POUR principle relates to keyboard navigation: perceivable or operable?"

```text
POUR
P - Perceivable: users can access the content
O - Operable: users can use the interface
U - Understandable: users can understand the content and actions
R - Robust: content works with different browsers and assistive technologies
```

## 20. Accessible Images Using Alt Text

Simple explanation:
Alt text describes the purpose or content of an image for users who cannot see it.

Real-world analogy:
Alt text is like a helpful person explaining what is important in a picture.

Real tech example:
On an Amazon product page, image alt text can help a screen reader user understand what the product looks like.

What to say to students:
"Good alt text is not about describing every pixel. It explains the useful meaning of the image."

Quick student question:
"What alt text would you write for a photo of a chocolate cake on a cafe menu?"

```html
<img src="cake.jpg" alt="Slice of chocolate cake on a white plate">
```

## 21. Accessible Forms Using Label And Input

Simple explanation:
Labels explain what each form input is for. The `for` attribute on the label should match the `id` on the input.

Real-world analogy:
A form without labels is like a set of blank boxes with no instructions.

Real tech example:
Revolut and Monzo forms must clearly label fields such as name, email and security details.

What to say to students:
"A placeholder is not a proper replacement for a label."

Quick student question:
"Why is a visible label useful even for users who do not use screen readers?"

```html
<label for="email">Email address</label>
<input id="email" name="email" type="email">
```

## 22. Colour Contrast And Not Using Colour Alone

Simple explanation:
Text must have enough contrast against its background. Important information should not depend only on colour.

Real-world analogy:
If a warning sign is too faint to read, it fails even if the words are correct.

Real tech example:
BBC breaking news banners use strong contrast and text labels, not just colour changes.

What to say to students:
"Colour can support meaning, but it should not be the only way meaning is communicated."

Quick student question:
"If an error is shown only by a red border, who might miss it?"

## 23. Keyboard Accessibility

Simple explanation:
Keyboard accessibility means users can navigate and operate the page using keys such as Tab, Enter and Space.

Real-world analogy:
A shop should have more than one usable entrance.

Real tech example:
GOV.UK services are designed so forms and links can be used without a mouse.

What to say to students:
"Try pressing Tab through a page. If you get lost, a keyboard user gets lost too."

Quick student question:
"Why might someone use a keyboard instead of a mouse?"

## 24. CSS Validation

Simple explanation:
CSS validation checks whether CSS follows standard syntax. The W3C CSS Validator helps find missing braces, invalid properties and typing mistakes.

Real-world analogy:
Validation is like spellcheck for code structure.

Real tech example:
Professional teams use automated checks so bugs are caught early before users see them.

What to say to students:
"Validation will not make your design beautiful, but it helps confirm the code is written correctly."

Quick student question:
"What kind of bug might happen if a CSS brace is missing?"

Validator:

- <https://jigsaw.w3.org/css-validator/>

## 25. Live Demo Plan

1. Create `index.html` with a cafe menu structure.
2. Link `style.css` using `<link rel="stylesheet" href="style.css">`.
3. Add body styles: font, background and margin reset.
4. Create a centered menu card.
5. Style headings and add a divider.
6. Add menu rows with item names and prices.
7. Use a class for repeated rows.
8. Add one ID for a unique section.
9. Demonstrate padding, margin and border.
10. Add a hover effect.
11. Add a mobile media query.
12. Link `print.css` and preview print styles.
13. Run the CSS through the W3C CSS Validator.
14. Ask students what accessibility improvements they can spot.

## 26. Questions To Ask Students

- What does CSS control that HTML does not?
- Why do professional sites prefer external CSS?
- When would you use a class instead of an ID?
- Which has more specific targeting: `.price` or `p`?
- What is the difference between margin and padding?
- Why does responsive design matter for a cafe menu?
- What does alt text help with?
- Why should forms use labels?
- What is one example of not relying on colour alone?
- What does the W3C CSS Validator check?

## 27. End-Of-Lecture Summary

Simple closing explanation:
CSS turns structured HTML into usable, attractive and responsive interfaces. Accessibility ensures those interfaces work for as many people as possible.

What to say to students:
"Today you learned how websites move from plain documents to real user interfaces. Next, you will practise by styling a modern cafe menu, validating the CSS and checking that the page works for different users and devices."

Key takeaways:

- HTML is structure; CSS is presentation; JavaScript is behaviour.
- CSS rules use selectors and declarations.
- Classes are reusable; IDs are unique.
- The cascade and specificity decide which styles win.
- Spacing, fonts, colours and layout affect usability.
- Responsive design supports different screen sizes.
- Print CSS supports paper output.
- Accessibility is a core part of professional front-end work.
- Validation helps catch CSS mistakes early.
