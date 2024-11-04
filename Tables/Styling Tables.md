# Styling Tables in HTML

Tables are used to display data in a structured format. Proper styling enhances the readability and presentation of tabular data, making it more appealing and easier to navigate.

#### 1. Basic Structure of a Table

An HTML table is created using the `<table>` element, with various other elements to define its structure:

- `<thead>`: Defines the header section of the table.
- `<tbody>`: Contains the main content of the table.
- `<tfoot>`: Defines the footer section of the table.
- `<tr>`: Represents a table row.
- `<th>`: Defines a header cell in a table.
- `<td>`: Represents a standard cell in a table.

**Basic Syntax**:
```html
<table>
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </tbody>
</table>
```

#### 2. Basic CSS for Styling Tables

You can use CSS to style tables for better visual appeal. Here are some common styling techniques:

##### a. Adding Borders
```css
table {
    border-collapse: collapse; /* Merges borders for a cleaner look */
}

th, td {
    border: 1px solid #ddd; /* Adds a light gray border to cells */
    padding: 8px;           /* Adds space inside cells */
}
```

##### b. Alternating Row Colors
Using CSS to create alternating row colors improves readability.
```css
tr:nth-child(even) {
    background-color: #f2f2f2; /* Light gray for even rows */
}

tr:hover {
    background-color: #ddd; /* Light gray on hover */
}
```

##### c. Header Styling
Make header cells visually distinct.
```css
th {
    background-color: #4CAF50; /* Green background for header */
    color: white;              /* White text color */
    text-align: left;          /* Align text to the left */
}
```

##### d. Text Alignment
Control text alignment within cells.
```css
td {
    text-align: center; /* Center-align text in standard cells */
}

th {
    text-align: left;   /* Left-align text in header cells */
}
```

##### e. Responsive Tables
Use CSS to make tables responsive on smaller screens.
```css
table {
    width: 100%; /* Full width of the container */
    overflow-x: auto; /* Allows horizontal scrolling */
    display: block; /* Make the table block-level */
}

th, td {
    white-space: nowrap; /* Prevent text wrapping */
}
```

#### 3. Advanced CSS Techniques

##### a. Using CSS Grid
You can create complex table layouts using CSS Grid for more control over styling.
```css
table {
    display: grid; /* Use grid layout */
    grid-template-columns: repeat(3, 1fr); /* Define three equal columns */
}
```

##### b. Media Queries
Use media queries to adjust table styles for different screen sizes.
```css
@media (max-width: 600px) {
    table {
        display: block; /* Stack the table */
    }
    th, td {
        display: block; /* Stack cells */
        text-align: right; /* Align text to the right */
    }
}
```

#### 4. Best Practices

1. **Keep It Simple**: Avoid excessive styling that can make tables harder to read.
2. **Maintain Consistency**: Use consistent colors, fonts, and padding throughout the table.
3. **Use Semantic HTML**: Always use the appropriate tags like `<th>`, `<tr>`, `<td>`, etc., for better accessibility and SEO.
4. **Ensure Responsiveness**: Design tables to be responsive for mobile devices, either through CSS or using frameworks like Bootstrap.

#### 5. Example of a Styled Table

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Table Example</title>
    <style>
        table {
            width: 100%;
            border-collapse: collapse;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #4CAF50;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        tr:hover {
            background-color: #ddd;
        }
    </style>
</head>
<body>
    <table>
        <thead>
            <tr>
                <th>Name</th>
                <th>Age</th>
                <th>City</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>John Doe</td>
                <td>30</td>
                <td>New York</td>
            </tr>
            <tr>
                <td>Jane Smith</td>
                <td>25</td>
                <td>Los Angeles</td>
            </tr>
            <tr>
                <td>Mike Johnson</td>
                <td>40</td>
                <td>Chicago</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

### Summary of Key Concepts

- **Basic Table Structure**: Use `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, and `<td>` to create a table.
- **CSS Styling**: Apply borders, background colors, padding, and text alignment to enhance table appearance.
- **Advanced Techniques**: Use CSS Grid for layout control and media queries for responsive design.
- **Best Practices**: Keep styling simple, maintain consistency, and ensure tables are accessible and responsive.

By following these notes, you can effectively style tables in HTML to improve their presentation and usability.