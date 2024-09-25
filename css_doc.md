# 1. Introduction to CSS

What is CSS?
CSS (Cascading Style Sheets) is used to control the look and feel of web pages.

CSS Syntax:

```css
selector {
  property: value;
}
```

```html
Ways to Include CSS in HTML:

Inline CSS:
<h1 style="color:blue;">Hello World</h1>
Internal CSS:
Defined inside <style> tags within the HTML file.
External CSS:
Linking an external CSS file using <link> tag.
CSS Preprocessors:
SCSS, SASS, LESS, etc.
```

# 2. CSS Selectors

```css
 Basic Selectors:

Element Selector (h1 {}).
Class Selector (.class {}).
ID Selector (#id {}).
Universal Selector (* {}).
Combinators:

Descendant Selector (div p {}).
Child Selector (div > p {}).
Adjacent Sibling Selector (h1 + p {}).
General Sibling Selector (h1 ~ p {}).
```

### Pseudo-classes:

```css

Hover: a:hover { color: red; }
Focus: input:focus { background-color: yellow; }
nth-child: li:nth-child(2) { color: blue; }

Pseudo-elements:

::before
::after
::first-letter
::first-line

```

# 3. Box Model

```css
Box Model Components:

Content: The actual content of the box (text, images).
Padding: Space between the content and the border.
Border: Surrounds the padding.
Margin: Space outside the border.

Box-sizing:

box-sizing: content-box;
box-sizing: border-box; (includes padding and border in width/height calculation).

```

# 4. CSS Layout

## Display Property:

```css

block, inline, inline-block, none
Positioning:

static, relative, absolute, fixed, sticky
Float and Clear:

float: left;
float: right;
Clearing floats using clear: both;
```

## Flexbox:

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

Flex Direction (row, column).
Justify Content (center, space-around, space-between).
Align Items (flex-start, center, flex-end).
```

## CSS Grid

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

Grid Template Columns/Rows.
Grid Gap.
Grid Areas.
```

# 5. CSS Units

```css
Absolute Units:
px, pt, cm, mm

Relative Units:

em: Relative to the font size of the element.
rem: Relative to the font size of the root element.
%: Percentage relative to the parent element.

```

# 6. Responsive Web Design

## Media Queries:

```css
@media (max-width: 600px) {
  .container {
    flex-direction: column;
  }
}

Mobile-First Design: Designing with small screens in mind first and then scaling up for larger screens using media queries.
```

## Viewport Meta Tag:

```css
<meta name="viewport" content="width=device-width, initial-scale=1.0">

```

# 7. CSS Animations and Transitions

## CSS Transitions:

```css
.box {
  transition: background-color 0.5s ease;
}
.box:hover {
  background-color: red;
}
```

## CSS Animations:

```css
@keyframes example {
  from { background-color: red; }
  to { background-color: yellow; }
}
.box {
  animation: example 5s infinite;
}

Animation Properties:

animation-duration
animation-name
animation-iteration-count

```

# 8. CSS Variables (Custom Properties)

## Declaring Variables:

```css
:root {
  --main-color: #3498db;
}
.box {
  background-color: var(--main-color);
}

Using Variables:

var(--main-color);
```

# 9. CSS Best Practices

## Avoid Inline CSS:

Use external or internal styles for better maintainability.

## Use Shorthand Properties:

Combine multiple CSS properties into one shorthand (e.g., margin, padding, background, font).

## Minimize Repaints and Reflows:

Avoid frequent changes to layout properties like width, height, and padding.

## BEM (Block, Element, Modifier) Naming Convention:

```css
.block__element--modifier {
  /* styles */
}
```

# 10. Advanced CSS Concepts

## CSS Specificity:

Calculating specificity (inline styles > IDs > classes > elements).

## CSS Inheritance:

Some properties like color, font-family, and text-align are inherited from the parent element.
Z-index:

Determines the stacking order of elements (z-index: 1;).

## CSS Sprites:

Combining multiple images into a single image file to improve loading speed and reduce the number of server requests.

# 11. CSS Frameworks

## Bootstrap:

Popular CSS framework for responsive design.
Grid system, components, and utility classes.

## Tailwind CSS:

Utility-first CSS framework.
No need for writing custom CSS; apply utility classes to elements.

# 12. CSS Performance Optimization

## Minify CSS Files:

Remove unnecessary whitespace and comments to reduce file size.

## Combine CSS Files:

Reduce the number of HTTP requests by combining multiple CSS files.

## Lazy Loading:

Load CSS only when needed to improve the page's loading speed.

## Use Gzip Compression:

Enable Gzip compression on the server to reduce file size.
