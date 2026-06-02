# COM109 Week 2 Lab – Styling a Modern Cafe Menu with CSS

## 1. Lab Objective

In this lab, you will style a modern cafe menu using CSS. The design is inspired by simple cafe menu examples, but you will make it more professional, responsive and accessible.

By the end of the lab, you should be able to:

- Link an external CSS file to an HTML page.
- Style the `body`, headings, sections and menu rows.
- Use classes and IDs.
- Apply margin, padding and borders.
- Align menu item names and prices.
- Add a hover effect.
- Add a responsive media query.
- Link a print stylesheet.
- Check CSS using the W3C CSS Validator.

## 2. Tools Needed

- Visual Studio Code or another code editor
- A web browser
- The W3C CSS Validator: <https://jigsaw.w3.org/css-validator/>
- The Week 2 starter files

## 3. Folder Structure

```text
WEEK2/
└── lab/
    ├── README.md
    ├── starter/
    │   ├── index.html
    │   └── style.css
    └── solution/
        ├── index.html
        ├── style.css
        └── print.css
```

## 4. What Students Will Build

You will build a one-page cafe menu for a fictional cafe. The page will include:

- A cafe name and subtitle
- Coffee items
- Dessert items
- Student specials
- Prices aligned neatly
- A footer with contact information
- Responsive styling for smaller screens
- Print-friendly styling

## 5. Step-By-Step Lecturer Demo

Follow this sequence with the class before students customise their own versions.

1. Open the starter `index.html`.
2. Show the HTML structure: `header`, `main`, `section` and `footer`.
3. Add the stylesheet link in the `<head>` if it is not already present.
4. Open `style.css` and add a body rule.
5. Set a font stack such as `Arial, Helvetica, sans-serif`.
6. Add a background colour or simple gradient.
7. Create a centered menu container using width, max-width and margin.
8. Add padding, border and background colour to the menu card.
9. Style the main heading and subtitle.
10. Add a horizontal divider.
11. Create menu item rows using a reusable class.
12. Use flexbox to place item names on the left and prices on the right.
13. Add a hover effect to make rows feel interactive.
14. Add an ID to one unique section and style it lightly.
15. Add a media query for screens below 600px.
16. Explain how `print.css` is linked in the solution.
17. Validate the CSS with the W3C CSS Validator.

## 6. Student Task

Starting with the files in `starter`, complete the cafe menu page.

Your page should include:

- A linked external stylesheet.
- A styled page background.
- A centered menu card or container.
- At least three menu sections.
- At least three items in each section.
- Prices aligned to the right.
- At least one class used more than once.
- At least one ID used for a unique section.
- Margin, padding and border rules.
- A hover effect on menu rows.
- A responsive media query.
- Valid CSS.

## 7. Challenge Tasks

Choose two or more:

- Change the cafe name.
- Change the menu items and prices.
- Add a desserts or snacks section.
- Change the colour palette while keeping good contrast.
- Add accessible alt text if you include an image.
- Add a contact section with opening times.
- Make the layout more comfortable on mobile.
- Add a print stylesheet.
- Validate both screen and print CSS.

## 8. Accessibility Checklist

Before submitting, check:

- The page has a meaningful title.
- Headings are in a sensible order.
- Text has good contrast against the background.
- Links use clear text.
- Information is not explained by colour alone.
- Images have meaningful `alt` text, if images are used.
- Forms have labels, if forms are added.
- The page can be navigated using the keyboard.

## 9. Responsive Design Checklist

Test the page by resizing the browser window.

- The menu should not be too wide on large screens.
- Text should remain readable on mobile.
- Menu rows should not overlap.
- Prices should remain easy to read.
- Padding should reduce on smaller screens if needed.
- The page should not require horizontal scrolling.

## 10. CSS Validation Task

1. Open <https://jigsaw.w3.org/css-validator/>.
2. Choose "By direct input" or upload your CSS file.
3. Paste your CSS.
4. Run the validator.
5. Fix any errors.
6. Re-run the validator until no errors remain.

Remember: the validator checks syntax. You still need to judge whether the design is readable, responsive and accessible.

## 11. Reflection Questions

- What part of CSS felt most useful today?
- What is the difference between a class and an ID?
- How did margin and padding change your design?
- What did the media query improve?
- What accessibility improvement are you most confident about?
- What did the CSS Validator help you find?
