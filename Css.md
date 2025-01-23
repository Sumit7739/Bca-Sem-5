
---

### **What is CSS?**

- **CSS (Cascading Style Sheets)** is used to style the appearance of an HTML page. It controls the layout, colors, fonts, margins, and more.
- It "cascades," meaning the most specific styles are applied when there are conflicts (e.g., inline styles override external ones).

---

### **CSS Creation**

There are three ways to use CSS:

1. **Inline CSS**: Add styles directly inside an HTML tag.
    
    ```html
    <p style="color: blue; font-size: 16px;">This is inline CSS</p>
    ```
    
2. **Internal CSS**: Define styles inside a `<style>` block in the `<head>` of the HTML page.
    
    ```html
    <head>
      <style>
        p {
          color: red;
          font-size: 18px;
        }
      </style>
    </head>
    ```
    
3. **External CSS**: Use a separate `.css` file and link it to your HTML page.
    
    - **HTML**:
        
        ```html
        <link rel="stylesheet" href="styles.css">
        ```
        
    - **CSS (styles.css)**:
        
        ```css
        p {
          color: green;
          font-size: 20px;
        }
        ```
        

---

### **Font in CSS**

CSS controls the font style, size, weight, and family:

- Example:
    
    ```css
    p {
      font-family: Arial, sans-serif; /* Font type */
      font-size: 16px;               /* Font size */
      font-weight: bold;             /* Font weight: normal, bold, or lighter */
      font-style: italic;            /* Font style: normal or italic */
    }
    ```
    

---

### **Color in CSS**

CSS allows you to set colors for text, background, and borders using keywords, HEX, RGB, or HSL values.

- Example:
    
    ```css
    body {
      color: blue;                  /* Text color */
      background-color: #f0f0f0;    /* Background color */
      border: 2px solid red;        /* Border color */
    }
    ```
    

---

### **Margin in CSS**

Margins add space **outside** an element (like padding adds space inside).

- Example:
    
    ```css
    div {
      margin: 20px;      /* Space around all sides */
      margin-top: 10px;  /* Space above */
      margin-right: 15px;/* Space to the right */
      margin-bottom: 10px;
      margin-left: 15px;
    }
    ```
    

---

### **List in CSS**

You can style **lists** (ordered `<ol>` or unordered `<ul>`).

- Example:
    
    ```css
    ul {
      list-style-type: square; /* Change bullet style (circle, square, none) */
      margin: 20px;            /* Add margin around the list */
      padding: 10px;           /* Space inside the list box */
      color: darkblue;         /* Color of the text */
    }
    li {
      font-size: 18px;         /* Style individual list items */
    }
    ```
    

---

### **Additional Notes**

- CSS simplifies the design process by separating style from content.
- CSS rules follow this structure:
    
    ```css
    selector {
      property: value;
    }
    ```
    
    Example:
    
    ```css
    h1 {
      color: red;
      text-align: center;
    }
    ```
    

---

Next -> [[Cgi and Perl]]