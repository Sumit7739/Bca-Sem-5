
---

### **SGML and HTML: Introduction**

- **SGML (Standard Generalized Markup Language)**: Think of SGML as the "parent" of all markup languages. It’s like a set of rules used to define different types of document structures (like HTML, XML, etc.).
- **HTML (HyperText Markup Language)**: HTML is a simpler "child" of SGML. It’s used to create and design web pages by structuring content, like text, images, and links.

---

### **HTML Page Structure**

An HTML page is like a blueprint for a web page. It has:

1. **`<!DOCTYPE html>`**: Tells the browser you’re using HTML5.
2. **`<html>`**: The root of the HTML document.
3. **`<head>`**: Contains information like the page title and metadata (things the user doesn’t directly see).
4. **`<body>`**: Contains the content you see on the page, like text, images, and links.

---

### **Text Formatting**

HTML has tags to format text. Some examples:

- **`<b>`**: Makes text bold.
- **`<i>`**: Makes text italic.
- **`<u>`**: Underlines the text.
- **`<p>`**: Creates a paragraph.
- **`<br>`**: Adds a line break (moves text to the next line).

---

### **Headings**

Headings in HTML are like titles and subtitles.

- Tags: **`<h1>`** to **`<h6>`**.
- **`<h1>`** is the largest and most important heading, while **`<h6>`** is the smallest.

---

### **Drawing Style (Text Style)**

You can apply styles to text using HTML attributes or CSS (Cascading Style Sheets). Examples:

- **Font color**: `<font color="red">Text</font>`
- **Font size**: `<font size="5">Text</font>` But nowadays, using **CSS** is preferred for styling.

---

### **List Creation**

Lists organize content neatly. Types:

1. **Ordered List (`<ol>`)**: Adds numbers (1, 2, 3...).
    
    ```html
    <ol>
      <li>First Item</li>
      <li>Second Item</li>
    </ol>
    ```
    
2. **Unordered List (`<ul>`)**: Adds bullet points.
    
    ```html
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
    </ul>
    ```
    

---

### **Graphics Tag**

For adding images, you use the `<img>` tag.

- Example: `<img src="image.jpg" alt="Description of image">`
- **`src`**: The file path or link to the image.
- **`alt`**: Text displayed if the image doesn’t load.

---

### **Table**

Tables help organize data in rows and columns.

- Example:
    
    ```html
    <table border="1">
      <tr>
        <th>Header 1</th>
        <th>Header 2</th>
      </tr>
      <tr>
        <td>Row 1, Col 1</td>
        <td>Row 1, Col 2</td>
      </tr>
    </table>
    ```
    
- **`<tr>`**: Table row.
- **`<td>`**: Table data (cell).
- **`<th>`**: Table header (bold and centered).

---

### **Colspan & Rowspan**

These are used to merge cells in a table.

- **`colspan`**: Merges cells horizontally (across columns).
    
    ```html
    <td colspan="2">Merged Cell</td>
    ```
    
- **`rowspan`**: Merges cells vertically (across rows).
    
    ```html
    <td rowspan="2">Merged Cell</td>
    ```
    

---

### **Linking Documents**

Links are created using the `<a>` tag.

- **External Linking**: Links to another website.
    
    ```html
    <a href="https://example.com">Go to Example</a>
    ```
    
- **Internal Linking**: Links to another part of your website.
    
    ```html
    <a href="about.html">About Us</a>
    ```
    

---

### **Frames & Frameset**

Frames allow you to divide a web page into sections, each showing a different web page. (This is outdated and not used much anymore.)

- **Frameset**: Defines the structure of the frames.
- **Example**:
    
    ```html
    <frameset cols="50%,50%">
      <frame src="page1.html">
      <frame src="page2.html">
    </frameset>
    ```
    

---

### **Marquee**

The `<marquee>` tag creates scrolling text or images (but it’s outdated now).

- Example:
    
    ```html
    <marquee>Welcome to my website!</marquee>
    ```
    

The text will scroll horizontally or vertically.

---

Next -> [[Css]]