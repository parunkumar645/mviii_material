1. Introduction to HTML
   HTML (HyperText Markup Language) is the standard language for creating web pages.
   It is used to structure content on the web and is composed of elements enclosed in tags.
   A basic HTML document starts with <!DOCTYPE html> declaration, which defines the document type and version of HTML.
   Basic Structure of an HTML document:
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Document</title>
     </head>
     <body>
       <h1>Hello, World!</h1>
     </body>
   </html>

2. HTML Elements
   HTML is made up of elements. An element is everything from the start tag to the end tag:
   <tagname>Content</tagname>
   Elements can contain:
   Attributes: Extra information about an element (e.g., id, class, src, href).
   Nested Elements: One element inside another.

3. HTML Headings and Paragraphs
Headings: Ranges from <h1> (largest) to <h6> (smallest).
Paragraphs: Represented using the <p> tag.
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<p>This is a paragraph.</p>

4. HTML Links
   Links are created using the <a> tag, where href specifies the destination URL.
   <a href="https://www.google.com" target="_blank">Visit Google</a>
   target="blank" opens the link in a new tab.

5. HTML Lists
Two main types of lists:
Ordered List (<ol>): List items are numbered.
Unordered List (<ul>): List items use bullet points.
<ol>
  <li>First item</li>
  <li>Second item</li>
</ol>

<ul>
  <li>Apple</li>
  <li>Banana</li>
</ul>

6. HTML Images
   Images are added using the <img> tag.
   Attributes include:
   src: The path of the image.
   alt: Alternative text if the image doesn't load.
   <img src="image.jpg" alt="Description of image" width="500" height="300">

7. HTML Tables
Tables are created using the <table> tag with rows (<tr>), table headers (<th>), and table data (<td>).
<table border="1">
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>

8. HTML Forms
   Forms are used to collect user input.

Important elements inside a form:

<input>: To take user input (text, radio, checkbox, etc.).
<label>: Label for form controls.
<select>: Dropdown list.
<textarea>: Multiline text input.

<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <input type="submit" value="Submit">
</form>

9. HTML Semantic Elements
   Semantic elements clearly describe their meaning:

<header>, <nav>, <section>, <article>, <footer>, <aside>, etc.

<header>
  <h1>Website Title</h1>
</header>
<section>
  <article>
    <h2>Article Title</h2>
    <p>This is some content.</p>
  </article>
</section>
<footer>Contact info</footer>

10. HTML Forms Input Types
    Forms can have various input types:
    Text: <input type="text">
    Password: <input type="password">
    Email: <input type="email">
    Radio buttons: <input type="radio">
    Checkboxes: <input type="checkbox">
    Submit button: <input type="submit">

11. HTML Attributes
    Attributes provide additional information about an element.
    Common attributes:
    id: Unique identifier.
    class: Class name(s) for CSS styling.
    href: For links.
    src: For images.
    style: Inline CSS styles.

12. HTML Audio and Video
    Audio: Embed audio files using <audio>.

Video: Embed video files using <video>.
<audio controls>

  <source src="audio.mp3" type="audio/mp3">
  Your browser does not support the audio element.
</audio>

<video controls>
  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

13. HTML Forms Validation
    Use the required attribute for mandatory fields.
    pattern attribute can be used for input validation (e.g., email or phone number format).

14. HTML5 New Features
    Canvas: For drawing graphics on the fly using JavaScript
    Geolocation API: To locate a user's geographical position.
    Local Storage: Store data in the user's browser that persists even after the browser is closed.

15. Meta Tags
Provide metadata about the HTML document.
Important tags:
<meta charset="UTF-8">: Defines the character encoding.
<meta name="description" content="Page description">: Describes the page for SEO.
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Responsive design.
