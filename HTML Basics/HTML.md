# What is HTML?

HTML (HyperText Markup Language) is the standard markup language used to create and design documents on the World Wide Web. It describes the structure of web pages using a series of elements or tags, which define various parts of the content such as headings, paragraphs, links, images, and other multimedia.

Key Characteristics of HTML:
- **Markup Language**: HTML uses tags to define elements, which browsers interpret to display the content.
- **Structure**: HTML provides the basic structure for web pages, which can be enhanced with CSS (Cascading Style Sheets) for styling and JavaScript for interactivity.
- **Hyperlinking**: HTML allows for the creation of hyperlinks, enabling navigation between different web pages or sites.
- **Multimedia Support**: HTML supports various multimedia elements, including images, audio, and video.

### Subtopics and Details with Examples

#### 1. Basic Structure of an HTML Document
An HTML document consists of several fundamental elements that define its structure.

**Example of a Simple HTML Document:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First HTML Page</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is my first HTML document.</p>
</body>
</html>
```
- **`<!DOCTYPE html>`**: Declares the document type and version of HTML.
- **`<html>`**: Root element of the HTML document.
- **`<head>`**: Contains meta-information about the document (title, character set, links to stylesheets, etc.).
- **`<body>`**: Contains the content of the web page, which is displayed to users.

#### 2. HTML Elements and Tags
HTML uses elements to create various types of content on the web. An element typically consists of an opening tag, content, and a closing tag.

**Example of Common HTML Tags:**
```html
<p>This is a paragraph.</p>
<a href="https://www.example.com">This is a link.</a>
<img src="image.jpg" alt="Description of image">
```
- **Paragraph**: Defined by `<p>` tags.
- **Link**: The `<a>` tag creates hyperlinks, using the `href` attribute to specify the URL.
- **Image**: The `<img>` tag displays images, with the `src` attribute specifying the image source and `alt` providing a text description.

#### 3. Text Formatting Tags
HTML provides tags for text formatting to enhance readability and structure.

**Example of Text Formatting:**
```html
<strong>Bold Text</strong>
<em>Italicized Text</em>
<u>Underlined Text</u>
```
- **`<strong>`**: Represents strong importance (usually bold).
- **`<em>`**: Indicates emphasis (usually italicized).
- **`<u>`**: Underlines the text.

#### 4. Lists in HTML
HTML supports different types of lists: unordered lists, ordered lists, and description lists.

**Example of Lists:**
```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>

<ol>
    <li>First Item</li>
    <li>Second Item</li>
</ol>

<dl>
    <dt>Definition Term</dt>
    <dd>Definition Description</dd>
</dl>
```
- **Unordered List (`<ul>`)**: Creates a bullet point list.
- **Ordered List (`<ol>`)**: Creates a numbered list.
- **Description List (`<dl>`)**: Pairs terms with their definitions.

#### 5. Links and Navigation
Links are essential for navigation between web pages.

**Example of Links:**
```html
<a href="https://www.example.com" target="_blank">Visit Example.com</a>
```
- The `target="_blank"` attribute opens the link in a new tab.

#### 6. Images and Multimedia
HTML supports various multimedia elements to enrich web content.

**Example of an Image:**
```html
<img src="path/to/image.jpg" alt="A descriptive text">
```
- **`src`**: Specifies the path to the image.
- **`alt`**: Provides alternative text for accessibility.

**Example of Audio and Video:**
```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio tag.
</audio>

<video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

#### 7. Forms in HTML
Forms allow users to input data, which can be sent to a server for processing.

**Example of a Simple Form:**
```html
<form action="/submit" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name">
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
    
    <input type="submit" value="Submit">
</form>
```
- **`<form>`**: Wraps the form elements, with `action` defining where to send the data and `method` specifying the HTTP method.
- **Input Types**: Various types like `text`, `email`, `submit`, etc., allow different data entries.

#### 8. Semantic HTML
Semantic HTML involves using HTML markup that conveys meaning and structure to the content.

**Example of Semantic Elements:**
```html
<header>
    <h1>Welcome to My Website</h1>
</header>

<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
    </ul>
</nav>

<article>
    <h2>Article Title</h2>
    <p>This is a great article.</p>
</article>

<footer>
    <p>© 2024 My Website</p>
</footer>
```
- **Semantic elements** like `<header>`, `<nav>`, `<article>`, and `<footer>` improve accessibility and SEO by clearly defining content sections.

#### 9. Tables in HTML
Tables organize data in rows and columns.

**Example of a Table:**
```html
<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Age</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>John Doe</td>
            <td>30</td>
        </tr>
        <tr>
            <td>Jane Smith</td>
            <td>25</td>
        </tr>
    </tbody>
</table>
```
- **`<table>`**: Defines the table.
- **`<tr>`**: Defines a row.
- **`<th>`**: Defines a header cell.
- **`<td>`**: Defines a standard cell.

#### 10. HTML5 Features
HTML5 introduced new features and elements for modern web applications.

**Examples of HTML5 Features:**
- **New Semantic Elements**: `<section>`, `<nav>`, `<article>`, `<header>`, `<footer>`.
- **APIs**: Canvas for graphics, Geolocation for location-based services.
- **Form Enhancements**: New input types like `date`, `color`, and attributes like `placeholder`.

#### 11. Accessibility in HTML
Creating accessible web pages ensures that all users, including those with disabilities, can use them effectively.

**Key Accessibility Practices:**
- Use **`alt`** attributes for images.
- Ensure proper heading structure (`<h1>` to `<h6>`) for screen readers.
- Use semantic elements to convey meaning.

#### 12. Best Practices
Adhering to best practices helps maintain clean, efficient, and accessible HTML code.

**Best Practices:**
- Write valid HTML (use validators).
- Organize code with proper indentation.
- Use comments for clarity.
- Optimize images for faster loading times.

### Summary of Key Concepts
- **Markup Language**: HTML is the foundational language for web pages.
- **Document Structure**: Understanding the basic structure is crucial.
- **Text and Media**: HTML supports text formatting and multimedia elements.
- **Forms and Semantics**: Forms facilitate user input, and semantic HTML enhances readability and accessibility.
