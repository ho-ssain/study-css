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

---

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

---

## Lesson-3: CSS Colors

CSS colors are used to specify the color of text, backgrounds, borders, and other elements on a webpage. There are various ways to represent colors in CSS, including named colors, hexadecimal notation, RGB values, RGBA values, HSL values, and HSLA values. Let's discuss each of these:

1. **Named Colors**:

   - CSS provides a set of predefined color names that you can use directly in your stylesheets.
   - Examples: `red`, `blue`, `green`, `yellow`, `black`, `white`, `orange`, etc.
   - Example usage: `color: red;`, `background-color: blue;`

2. **Hexadecimal Notation**:

   - Colors can be represented using hexadecimal notation, which consists of a hash `#` followed by three or six hexadecimal digits (0-9, A-F).
   - The three-digit format represents RGB values in shorthand (e.g., `#f00` for red), and the six-digit format represents the full RGB color space (e.g., `#ff0000` for red).
   - Example usage: `color: #ff0000;`, `background-color: #00ff00;`

3. **RGB Values**:

   - RGB (Red, Green, Blue) notation represents colors using the intensities of the red, green, and blue components on a scale of 0 to 255.
   - Syntax: `rgb(redValue, greenValue, blueValue)`
   - Example usage: `color: rgb(255, 0, 0);`, `background-color: rgb(0, 255, 0);`

4. **RGBA Values**:

   - RGBA is similar to RGB, but with an additional alpha channel that specifies the opacity of the color (transparency), ranging from 0 (fully transparent) to 1 (fully opaque).
   - Syntax: `rgba(redValue, greenValue, blueValue, alphaValue)`
   - Example usage: `color: rgba(255, 0, 0, 0.5);`, `background-color: rgba(0, 255, 0, 0.75);`

5. **HSL Values**:

   - HSL (Hue, Saturation, Lightness) notation represents colors using the hue (color tone), saturation (color intensity), and lightness (brightness) components.
   - Hue is represented as an angle in degrees (0 to 360), while saturation and lightness are percentages (0% to 100%).
   - Syntax: `hsl(hue, saturation, lightness)`
   - Example usage: `color: hsl(0, 100%, 50%);`, `background-color: hsl(120, 100%, 50%);`

6. **HSLA Values**:
   - Similar to HSL, but with an additional alpha channel for specifying opacity.
   - Syntax: `hsla(hue, saturation, lightness, alpha)`
   - Example usage: `color: hsla(0, 100%, 50%, 0.5);`, `background-color: hsla(120, 100%, 50%, 0.75);`

By understanding these different color representations in CSS, you have the flexibility to choose the most suitable method based on your design requirements and preferences. Each notation has its advantages and use cases, allowing you to create visually appealing and harmonious color schemes for your webpages.

---

## Lesson-4: CSS Units

CSS units and sizes are used to define the dimensions, spacing, and positioning of elements on a webpage. They come in various types, each serving different purposes. Here's a brief overview of CSS units and sizes:

1. **Absolute Length Units**:

   - Absolute length units are fixed and do not change based on the viewport or device.
   - Examples:
     - `px` (pixels): Represents a single dot on a computer screen. Widely used for precise control over element sizes.
     - `in` (inches), `cm` (centimeters), `mm` (millimeters): Useful for print stylesheets, where physical measurements are required.
     - `pt` (points), `pc` (picas): Also used in print stylesheets, with 1 point equaling 1/72 of an inch, and 1 pica equaling 12 points.

2. **Relative Length Units**:

   - Relative length units are relative to another value, such as the font size or the size of the viewport.
   - Examples:
     - `em`: Represents the font size of the element itself. For example, `1em` is equal to the font size of the current element.
     - `rem`: Similar to `em`, but relative to the root element (`<html>`), making it more predictable.
     - `vw` (viewport width), `vh` (viewport height): Represents a percentage of the viewport width or height, respectively.
     - `vmin`, `vmax`: Represents the smaller or larger of `vw` and `vh`, respectively.

3. **Percentage Units**:

   - Percentage units are relative to another value, typically the parent element or the viewport.
   - Examples:
     - `%`: Represents a percentage of the parent element's size. For example, `50%` is half the size of the parent element.
     - `%`: Also used in conjunction with `vw` and `vh` to create responsive layouts based on the viewport size.

4. **Flexible Length Units**:

   - Flexible length units are based on a combination of absolute and relative values, allowing for more flexible and responsive layouts.
   - Examples:
     - `fr` (flex): Represents a fraction of the available space in a flex container. Used in CSS Flexbox layouts.
     - `ch`: Represents the width of the character "0" in the current font. Useful for aligning elements based on character width.

5. **Viewport-Percentage Units**:
   - Viewport-percentage units are relative to the size of the viewport, allowing for responsive designs based on the device's screen size.
   - Examples:
     - `vw` (viewport width): Represents a percentage of the viewport's width.
     - `vh` (viewport height): Represents a percentage of the viewport's height.
     - `vmin`, `vmax`: Represents the smaller or larger of `vw` and `vh`, respectively.

These CSS units and sizes provide flexibility and control over the layout and appearance of elements on a webpage. By understanding how to use them effectively, you can create responsive and visually appealing designs that adapt to different devices and screen sizes.

---

## Lesson-5: CSS Box Model

The CSS Box Model is a fundamental concept in CSS that describes the layout and rendering of elements on a webpage. It conceptualizes each HTML element as a rectangular box, comprising content, padding, borders, and margins. Here's a brief overview of the CSS Box Model:

1. **Content**:

   - The content area of an element represents the actual content, such as text, images, or other media, contained within the element.
   - The size of the content area is determined by the `width` and `height` properties specified in CSS.

2. **Padding**:

   - Padding is the space between the content area and the element's border.
   - It provides internal spacing within the element, separating the content from its borders.
   - Padding can be adjusted using the `padding` property in CSS, which accepts values in pixels, percentages, or other length units.

3. **Border**:

   - The border surrounds the padding area and visually separates the element's content from its surroundings.
   - Borders can have different styles (solid, dashed, dotted, etc.), widths, and colors.
   - Border properties include `border-width`, `border-style`, and `border-color`, among others.

4. **Margin**:
   - Margin is the space outside the element's border, separating it from other elements in the layout.
   - It creates space between adjacent elements, preventing them from visually merging.
   - Margins can be adjusted using the `margin` property in CSS, which accepts values in pixels, percentages, or other length units.

The total space occupied by an element, including its content, padding, border, and margin, is referred to as the "box" of the element. The size of the box is calculated as follows:

```css
Total width = width + padding-left + padding-right + border-left-width + border-right-width + margin-left + margin-right
Total height = height + padding-top + padding-bottom + border-top-width + border-bottom-width + margin-top + margin-bottom
```

Understanding the CSS Box Model is essential for accurately controlling the layout, spacing, and appearance of elements on a webpage. By adjusting the content, padding, borders, and margins of elements, designers and developers can create visually appealing and well-structured layouts that adapt to various screen sizes and devices.

---

## Lesson-6: Typography

Typography in web design refers to the art and technique of arranging type to make written language legible, readable, and visually appealing when displayed on a screen. It plays a crucial role in user experience and can significantly impact how content is perceived and understood by users. Here are some key aspects of typography in web design:

1. **Font Selection**:

   - Choosing the right fonts sets the tone and personality of a website. There are two main types of fonts: serif and sans-serif. Serif fonts have decorative strokes at the ends of characters, while sans-serif fonts do not. Each type conveys a different aesthetic and mood.
   - Web designers often select fonts that complement the website's brand identity and reflect its content and audience. It's essential to consider factors such as readability, legibility, and accessibility when choosing fonts for web typography.

2. **Font Size and Hierarchy**:

   - Establishing a clear hierarchy of font sizes helps users navigate and understand the content more easily. Headings (h1-h6) should be larger and bolder than body text to signify importance and structure.
   - Responsive web design techniques ensure that font sizes adjust appropriately across different screen sizes and devices, providing a consistent reading experience for users.

3. **Line Length and Spacing**:

   - The length of lines (line length) and the spacing between lines (line height) affect readability. Optimal line length typically ranges from 50 to 75 characters per line to prevent eye strain and maintain focus.
   - Adequate line spacing ensures that text is comfortably readable. Line height is typically set to 1.5-1.6 times the font size to provide enough space between lines without overcrowding or causing text to appear disjointed.

4. **Typography Scale**:

   - A typography scale consists of a series of font sizes that follow a consistent ratio or progression. Modular scales, such as the golden ratio or the typographic scale, help maintain harmony and balance in typography across a website.
   - Using a typography scale ensures that font sizes are proportionally related, creating a visually pleasing and cohesive design.

5. **Typography Effects**:

   - Text styling effects, such as bold, italic, underline, and color changes, can be used to emphasize important information, create visual interest, and guide user attention.
   - Care should be taken to use these effects judiciously and consistently to maintain readability and avoid visual clutter.

6. **Accessibility**:
   - Accessibility considerations are essential in web typography to ensure that content is accessible to users with disabilities, including visual impairments.
   - Providing sufficient color contrast between text and background, using readable fonts, and allowing users to adjust font size are critical accessibility practices.

In summary, typography in web design encompasses font selection, size, hierarchy, spacing, and styling to create visually appealing and readable content. By employing principles of good typography, web designers can enhance the user experience, communicate effectively, and convey the intended message of the website.

---

## Lesson-7: Styling Links

Styling links in CSS is crucial for enhancing their visibility, usability, and aesthetic appeal. Links are a fundamental aspect of web navigation, and their appearance can greatly influence user experience. Here are some common techniques for styling links in CSS:

1. **Text Color**:

   - Set the color of the link text to distinguish it from surrounding content.
   - Use contrasting colors to ensure readability, especially against the background color.
   - Example: `a { color: blue; }`

2. **Text Decoration**:

   - Apply decorative effects to the link text, such as underlining or removing the default underline.
   - Common values for the `text-decoration` property include `underline`, `none`, `overline`, and `line-through`.
   - Example: `a { text-decoration: none; }`

3. **Hover Effects**:

   - Add visual feedback to links when users hover over them with the mouse pointer.
   - Change the color, underline, or background of the link to indicate interactivity.
   - Example: `a:hover { color: red; }`

4. **Visited Links**:

   - Style links that have been visited by users differently from unvisited links to provide visual feedback.
   - Use a distinct color or text decoration for visited links to help users keep track of their browsing history.
   - Example: `a:visited { color: purple; }`

5. **Active Links**:

   - Style links when they are being activated, such as when clicked.
   - Apply different colors or effects to indicate the active state of the link.
   - Example: `a:active { color: green; }`

6. **Focus Styles**:

   - Ensure links are easily identifiable and accessible when they receive keyboard focus.
   - Use a different color, border, or outline to highlight focused links.
   - Example: `a:focus { outline: 2px solid blue; }`

7. **Link States**:

   - Style links based on their states, such as `:hover`, `:visited`, `:active`, and `:focus`.
   - Use different styles for each state to provide clear visual feedback to users.
   - Example:

     ```css
     a:hover {
       color: red;
     }
     a:visited {
       color: purple;
     }
     a:active {
       color: green;
     }
     a:focus {
       outline: 2px solid blue;
     }
     ```

8. **Link Underlines**:
   - Control the appearance of link underlines, including their thickness, style, and color.
   - Customize underlines to match the overall design aesthetic of the website.
   - Example: `a { text-decoration: underline dotted blue; }`

By applying these styling techniques, you can create visually appealing and user-friendly links that enhance navigation and improve the overall experience of your website visitors.

---

## Lesson-8: List Styles

In CSS, list styles refer to the appearance of lists, including unordered lists (`<ul>`) and ordered lists (`<ol>`). You can control various aspects of list styling, such as the type of bullet or numbering, position, spacing, and appearance of list items. Here's a comprehensive overview of list styles in CSS:

1. **List Style Type**:

   - Determines the type of marker used for list items.
   - Common values for unordered lists (`<ul>`) include `disc`, `circle`, and `square`.
   - Common values for ordered lists (`<ol>`) include `decimal`, `lower-alpha`, and `upper-roman`.
   - Example:

     ```css
     ul {
       list-style-type: circle; /* Bullets as circles */
     }
     ol {
       list-style-type: decimal; /* Numbering as decimal */
     }
     ```

2. **List Style Position**:

   - Specifies the position of the marker relative to the list item text.
   - Values include `inside` (marker inside the list item box) and `outside` (marker outside the list item box).
   - Example:

     ```css
     ul {
       list-style-position: inside; /* Bullets inside the list item box */
     }
     ```

3. **List Style Image**:

   - Allows you to use custom images as list item markers.
   - Use the `url()` function to specify the path to the image.
   - Example:

     ```css
     ul {
       list-style-image: url("path/to/image.png"); /* Custom image as list item marker */
     }
     ```

4. **List Style Shorthand**:

   - The `list-style` shorthand property can be used to set all list style properties (type, position, image) in one declaration.
   - Example:

     ```css
     ul {
       list-style: square inside url("path/to/image.png"); /* Bullet as square, inside list item, with custom image */
     }
     ```

5. **List Item Styles**:

   - You can apply styles directly to list items (`<li>`), such as padding, margin, color, and background.
   - Example:

     ```css
     li {
       padding: 5px;
       margin-bottom: 10px;
       color: #333;
       background-color: #f5f5f5;
     }
     ```

6. **Nested Lists**:

   - Styles applied to parent lists can also affect nested lists. Use descendant selectors to target nested lists specifically.
   - Example:

     ```css
     ul ul {
       list-style-type: square; /* Nested lists have square bullets */
     }
     ```

By utilizing these CSS properties and techniques, you can customize the appearance of lists on your webpages to match the design and layout requirements of your site. Whether you're creating simple bulleted lists or complex numbered outlines, CSS provides the flexibility to tailor list styles to your needs.

## Lesson-9: Mini Project

---

## Lesson-10: Display

In CSS, the `display` property is used to control how an element is rendered in the document layout. It specifies the type of box model used for an element, which determines how it interacts with other elements in the document flow. The `display` property accepts various values, each with its own behavior. Here's an overview of some commonly used values for the `display` property:

1. **`block`**:

   - The element generates a block-level box, which typically starts on a new line and stretches to fill the width of its containing element.
   - Examples of block-level elements include `<div>`, `<p>`, `<h1>`-`<h6>`, `<ul>`, `<ol>`, `<li>`, and `<section>`.

2. **`inline`**:

   - The element generates an inline-level box, which does not start on a new line and only takes up as much width as necessary.
   - Examples of inline-level elements include `<span>`, `<a>`, `<strong>`, `<em>`, and `<img>`.

3. **`inline-block`**:

   - The element generates an inline-level box that behaves like a block-level box. It does not start on a new line but can have width, height, padding, and margins.
   - Useful for elements that need to be displayed inline but also require block-level styling, such as buttons or form elements.

4. **`none`**:

   - The element is removed from the document layout entirely. It does not occupy any space on the page, and its contents are not rendered.
   - Useful for hiding elements dynamically using JavaScript or CSS.

5. **`flex`**:

   - The element becomes a flex container, and its direct children become flex items. This allows for flexible layouts using the flexbox model.
   - Flex containers can be manipulated using properties like `justify-content`, `align-items`, and `flex-direction`.

6. **`grid`**:

   - The element becomes a grid container, and its direct children become grid items. This allows for complex layouts using the CSS Grid Layout module.
   - Grid containers can be manipulated using properties like `grid-template-columns`, `grid-template-rows`, and `grid-gap`.

7. **`table`, `table-cell`, `table-row`, `table-row-group`, etc.**:
   - These values generate elements that behave like HTML table elements. They are useful for creating table-like layouts without using actual `<table>` elements.

Understanding and appropriately using the `display` property is essential for controlling the layout and structure of webpages. By selecting the appropriate `display` value, you can achieve the desired visual presentation and ensure proper interaction between elements within your document layout.

---

## Lesson-11: Floats

## Resources adn tools

- [coolors](https://coolors.co/) is a great tool to generate colors based on specific
