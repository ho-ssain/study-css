# Study_CSS

![css](/imgs/css.png)

---

## Lesson-1: Start

### what is CSS?

CSS (Cascading Style Sheets) is a language used to control the presentation and styling of webpages written in HTML or XHTML. In simpler terms, CSS is what makes websites look good and visually appealing.

CSS:

1. **Styling Webpages**:

   - CSS is used to style the layout, colors, fonts, spacing, and overall appearance of elements on a webpage.
   - It allows you to change how text, images, links, buttons, and other HTML elements look and behave.

2. **Separation of Concerns**:

   - CSS allows for the separation of content (HTML) from presentation (CSS) and behavior (JavaScript).
   - This separation makes it easier to manage and update the styling of a website without having to change the underlying HTML structure.

3. **Selectors and Rules**:

   - CSS uses selectors to target HTML elements and apply styling rules to them.
   - For example, you can select all `<p>` elements and change their font size or select elements with a specific class and change their background color.

4. **Syntax**:

   - CSS rules consist of a selector, followed by a declaration block enclosed in curly braces `{}`.
   - Within the declaration block, you specify one or more property-value pairs separated by semicolons.
   - For example:

     ```css
     p {
       font-size: 16px;
       color: #333333;
     }
     ```

5. **Cascading and Specificity**:

   - CSS stands for "Cascading Style Sheets," which means that styles can cascade or flow from one element to another.
   - Specificity determines which styles take precedence when multiple conflicting styles are applied to the same element.

6. **Media Queries**:
   - CSS allows for responsive web design by using media queries to apply different styles based on the characteristics of the device, such as screen size, resolution, or orientation.
   - This enables websites to adapt and display optimally on various devices, including desktops, tablets, and smartphones.

In summary, CSS is a powerful language that controls the visual presentation of web content. It enables web designers and developers to customize the look and feel of websites, create engaging user experiences, and ensure compatibility across different browsers and devices.

### different ways of applying CSS to HTML

1. Basic Methods:
   - Inline Styles
   - Internal Styles
   - External Stylesheets
2. Advanced Methods:
   - CSS Frameworks
   - CSS-in-JS
   - Importing CSS in JavaScript Modules
   - Inline style Attribute in JSX (for React)

### Writing CSS

1. **Selector**:

   - A selector targets HTML elements that you want to style.
   - Selectors can be HTML elements, classes, IDs, attributes, or combinations of these.
   - Example selectors: `h1`, `.button`, `#header`, `[type="text"]`.

2. **Declaration Block**:

   - After the selector, you enclose the CSS declarations within curly braces `{}`.
   - Each declaration consists of a property and a value, separated by a colon `:`.
   - Multiple declarations are separated by semicolons `;`.
   - Example declaration block:

     ```css
     selector {
       property1: value1;
       property2: value2;
       /* more properties */
     }
     ```

## Lesson-2: Selectors

### Types of CSS Selectors

1. **Element Styles**:

   - Applying styles directly to HTML elements using element selectors.
   - Example:

     ```css
     h1 {
       color: blue;
       font-size: 24px;
     }
     ```

2. **Class Styles**:

   - Applying styles to elements with specific class names.
   - Example:

     ```css
     .button {
       background-color: #007bff;
       color: white;
       padding: 10px 20px;
     }
     ```

3. **ID Styles**:

   - Applying styles to elements with specific IDs.
   - Note: IDs should be unique within a document.
   - Example:

     ```css
     #header {
       background-color: #333;
       color: white;
       padding: 10px;
     }
     ```

4. **Attribute Styles**:

   - Applying styles to elements based on their attributes.
   - Example:

     ```css
     input[type="text"] {
       border: 1px solid #ccc;
       padding: 5px;
     }
     ```

5. **Pseudo-class Styles**:

   - Applying styles to elements based on their state or position.
   - Examples: `:hover`, `:active`, `:focus`, `:nth-child()`, etc.
   - Example:

     ```css
     button:hover {
       background-color: #ffcc00;
     }
     ```

6. **Pseudo-element Styles**:

   - Applying styles to parts of an element.
   - Examples: `::before`, `::after`, `::first-line`, `::first-letter`, etc.
   - Example:

     ```css
     p::first-line {
       font-weight: bold;
     }
     ```

7. **Grouping Styles**:

   - Grouping multiple selectors together to apply the same styles.
   - Example:

     ```css
     h1,
     h2,
     h3 {
       font-family: Arial, sans-serif;
     }
     ```

These are the main types of CSS rules or decorations we'll encounter when styling webpages. By understanding how to write CSS and the different ways to target elements, we can effectively style our HTML documents and create visually appealing websites.
