# Table Attributes

HTML tables are used to display data in a structured format, typically in rows and columns. Various attributes can be applied to tables to enhance their presentation and functionality. Below are the main table attributes, their definitions, and examples.

#### 1. `<table>` Attributes

- **`border`**: Specifies the width of the border around the table.
  - **Usage**: `<table border="1">` 
  - **Example**:
    ```html
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
    ```

- **`cellpadding`**: Defines the space between the cell content and its border.
  - **Usage**: `<table cellpadding="10">`
  - **Example**:
    ```html
    <table cellpadding="10">
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ```

- **`cellspacing`**: Specifies the space between individual cells in a table.
  - **Usage**: `<table cellspacing="5">`
  - **Example**:
    ```html
    <table cellspacing="5">
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ```

- **`width`**: Sets the width of the table. It can be specified in pixels or as a percentage of the containing element.
  - **Usage**: `<table width="100%">`
  - **Example**:
    ```html
    <table width="100%">
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ```

- **`height`**: Defines the height of the table.
  - **Usage**: `<table height="200">`
  - **Example**:
    ```html
    <table height="200">
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ```

#### 2. `<tr>`, `<th>`, and `<td>` Attributes

- **`align`**: Specifies the alignment of the content within the table row or cell. Possible values include `left`, `right`, and `center`.
  - **Usage**: `<tr align="center">`
  - **Example**:
    ```html
    <tr align="center">
        <th>Header</th>
        <th>Header</th>
    </tr>
    ```

- **`valign`**: Sets the vertical alignment of the content within the cell. Possible values include `top`, `middle`, and `bottom`.
  - **Usage**: `<td valign="top">`
  - **Example**:
    ```html
    <td valign="top">Data 1</td>
    ```

- **`colspan`**: Specifies the number of columns a cell should span.
  - **Usage**: `<td colspan="2">`
  - **Example**:
    ```html
    <tr>
        <td colspan="2">Merged Cell</td>
    </tr>
    ```

- **`rowspan`**: Defines the number of rows a cell should span.
  - **Usage**: `<td rowspan="2">`
  - **Example**:
    ```html
    <td rowspan="2">Merged Row</td>
    ```

#### 3. `<caption>` Attribute

- **`caption`**: Defines a title or caption for the table.
  - **Usage**: `<caption>Your Table Title</caption>`
  - **Example**:
    ```html
    <table>
        <caption>Monthly Sales Report</caption>
        <tr>
            <th>Month</th>
            <th>Sales</th>
        </tr>
        <tr>
            <td>January</td>
            <td>$5000</td>
        </tr>
    </table>
    ```

#### 4. Styling Tables with CSS

While HTML attributes can be used to style tables, it is often preferable to use CSS for better control over presentation.

- **Example of CSS for Tables**:
    ```html
    <style>
        table {
            width: 100%;
            border-collapse: collapse; /* Combines borders */
        }
        th, td {
            border: 1px solid black;
            padding: 10px;
            text-align: left;
        }
    </style>
    <table>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ```

### Summary

Table attributes play a vital role in defining the structure and presentation of data in HTML tables. Understanding how to use these attributes effectively can greatly enhance the readability and functionality of your tables, making them an essential tool for displaying data on the web. Utilizing CSS in conjunction with HTML attributes allows for more sophisticated designs and layouts, leading to a better user experience.