# HTML Headings

Headings in HTML are used to create a hierarchy of content, making it easier for users and search engines to understand the structure of a webpage. HTML provides six levels of headings, ranging from `<h1>` to `<h6>`.

#### 1. Structure of HTML Headings

- **`<h1>`:** Represents the main heading (highest level).
- **`<h2>`:** Represents a subheading of `<h1>`.
- **`<h3>`:** Represents a subheading of `<h2>`.
- **`<h4>`:** Represents a subheading of `<h3>`.
- **`<h5>`:** Represents a subheading of `<h4>`.
- **`<h6>`:** Represents the lowest level heading.

**Example:**
```html
<h1>Main Heading</h1>
<h2>Subheading Level 1</h2>
<h3>Subheading Level 2</h3>
<h4>Subheading Level 3</h4>
<h5>Subheading Level 4</h5>
<h6>Subheading Level 5</h6>
```

#### 2. Usage of Headings

- **Content Organization:** Headings help structure the content, making it easier for readers to navigate and understand the hierarchy of information.
- **SEO Benefits:** Search engines use headings to understand the topic and structure of a webpage, which can influence rankings.
- **Accessibility:** Properly used headings improve accessibility for screen readers, allowing visually impaired users to navigate the content more effectively.

#### 3. Best Practices for Using Headings

- **Use One `<h1>` per Page:** Generally, it’s best practice to have a single `<h1>` tag per page to indicate the main topic.
- **Follow a Hierarchical Structure:** Use headings in a logical order. For example, after an `<h1>`, use `<h2>` for main sections and `<h3>` for subsections.
- **Keep Headings Descriptive:** Use clear and descriptive text for headings to help users understand the content that follows.
- **Avoid Skipping Levels:** Do not skip heading levels (e.g., using `<h3>` before `<h2>`) as it can confuse both users and search engines.
- **Style with CSS:** Use CSS to style headings for better visual impact while maintaining semantic meaning.

#### 4. Example of Proper Headings Usage

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Headings Example</title>
</head>
<body>
    <h1>Understanding HTML Headings</h1>
    <h2>Introduction</h2>
    <p>This section introduces the concept of HTML headings.</p>
    
    <h2>Types of Headings</h2>
    <h3>Primary Heading</h3>
    <p>The <code>&lt;h1&gt;</code> tag is used for the main heading.</p>
    
    <h3>Secondary Headings</h3>
    <p>The <code>&lt;h2&gt;</code> to <code>&lt;h6&gt;</code> tags are used for subheadings.</p>
    
    <h2>Best Practices</h2>
    <p>Follow best practices to ensure proper usage of headings.</p>
</body>
</html>
```

#### 5. Summary of Key Concepts

- **Headings (`<h1>` to `<h6>`):** Used to create a structured hierarchy of content on a webpage.
- **Content Organization:** They help organize information for better readability and navigation.
- **SEO and Accessibility:** Proper use enhances SEO and accessibility for users with disabilities.

By effectively utilizing headings, you can create well-structured and accessible web pages that improve user experience and search engine optimization.