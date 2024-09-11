### Student Notes: Learning Web Blocks with AI

---

### **1. Introduction**

- **Objective:**
  - The goal of this session is to learn the basics of HTML and CSS, and how to use them together to create a simple web page.
  - We will also explore how effective prompts can help in learning and applying web technologies with AI tools.

---

### **2. Learning Basic HTML with AI**

- **Objective:** Understand and implement basic HTML tags.

  - **Introduction to HTML:**

    - **What is HTML?**
      - HTML stands for Hypertext Markup Language. It is used to structure content on the web.
    - **Prompts for Learning HTML:**

      - **Prompt for Basic Tags:**
        - "What are the basic HTML tags needed to create a simple web page? How are they used?"
        - **Example Answer:** Basic HTML tags include `<html>`, `<head>`, `<body>`, `<h1>`, `<p>`, `<a>`, and `<img>`. These tags structure content like headings, paragraphs, links, and images.
      - **Prompt for HTML Structure:**
        - "Can you explain the structure of a basic HTML document and how the `<head>` and `<body>` sections work?"
        - **Example Answer:** An HTML document has a `<head>` section for metadata (like title and links to stylesheets) and a `<body>` section for the main content.

    - **Implementation:**

      - **Creating an HTML Document:**
        - Write a simple HTML document with basic tags:
          ```html
          <!DOCTYPE html>
          <html>
            <head>
              <title>My First Web Page</title>
            </head>
            <body>
              <h1>Welcome to My Web Page</h1>
              <p>This is a paragraph of text.</p>
              <a href="https://www.example.com">Visit Example.com</a>
              <img src="image.jpg" alt="Example Image" />
            </body>
          </html>
          ```

    - **Cross-Questioning Prompts:**
      - **Prompt for Tag Purpose:**
        - "What is the purpose of the `<head>` section in an HTML document? What kind of information does it typically contain?"
      - **Prompt for Nesting Tags:**
        - "How does nesting HTML tags affect the layout and content structure of a web page?"

---

### **3. Learning CSS with AI**

- **Objective:** Understand and implement basic CSS styles.

  - **Introduction to CSS:**

    - **What is CSS?**
      - CSS stands for Cascading Style Sheets. It is used to style and layout web pages.
    - **Prompts for Learning CSS:**

      - **Prompt for Basic CSS Properties:**
        - "What are some fundamental CSS properties for styling text and layout? How are they applied?"
        - **Example Answer:** Basic CSS properties include `color`, `font-family`, `font-size`, `margin`, `padding`, and `border`.
      - **Prompt for CSS Selectors:**
        - "How do CSS selectors work to target specific HTML elements for styling?"
        - **Example Answer:** CSS selectors like class selectors (`.class`), ID selectors (`#id`), and element selectors (`element`) are used to apply styles to specific elements.

    - **Implementation:**

      - **Applying CSS Styles:**
        - Add CSS to style the HTML document:
          ```css
          body {
            font-family: Arial, sans-serif;
            color: #333;
          }
          h1 {
            color: #007bff;
          }
          p {
            margin: 20px 0;
            padding: 10px;
            border: 1px solid #ddd;
          }
          ```

    - **Cross-Questioning Prompts:**
      - **Prompt for Property Impact:**
        - "How does changing the `margin` and `padding` properties affect the layout of HTML elements?"
      - **Prompt for Selector Types:**
        - "What are the differences between class selectors and ID selectors in CSS? Provide examples of each."

---

### **4. Creating a Simple Web Page**

- **Objective:** Combine HTML and CSS knowledge to build a basic web page.

  - **Combining HTML and CSS:**

    - **Linking CSS to HTML:**

      - Use the `<link>` tag in the `<head>` section of your HTML document to include a CSS stylesheet.
      - **Example:**
        ```html
        <link rel="stylesheet" href="styles.css" />
        ```

    - **Using Prompts to Create a Web Page:**

      - **Prompt for Page Layout:**
        - "How do you create a basic layout for a web page using HTML and CSS? Include examples of elements like headings, paragraphs, images, and links."
        - **Example Answer:** Combine HTML elements and CSS styles to create a layout with headings, paragraphs, images, and links.
      - **Prompt for CSS Integration:**
        - "How do you apply a CSS stylesheet to an HTML document to style the page? What are the steps to link the stylesheet and use CSS rules?"

    - **Implementation:**

      - **Building a Web Page:**
        - Create a simple web page integrating HTML and CSS:
          ```html
          <!DOCTYPE html>
          <html>
            <head>
              <title>Styled Web Page</title>
              <link rel="stylesheet" href="styles.css" />
            </head>
            <body>
              <h1>My Styled Web Page</h1>
              <p>This paragraph is styled with CSS.</p>
              <a href="https://www.example.com">Visit Example.com</a>
              <img src="image.jpg" alt="Styled Image" />
            </body>
          </html>
          ```

    - **Interactive Demonstration:**

      - Show how HTML and CSS work together in a live demonstration. Implement a simple web page and apply styles to see changes in real-time.

    - **Cross-Questioning Prompts:**
      - **Prompt for Styling Impact:**
        - "How does applying CSS styles change the appearance of HTML elements? Provide examples of how different CSS properties affect element presentation."
      - **Prompt for Layout Design:**
        - "What are some common practices for designing a web page layout using HTML and CSS? How can you ensure that the layout is responsive?"

---

### **5. Closing**

- **Summary:**

  - Review the key concepts covered: basic HTML tags, CSS properties, and how to integrate both to create a styled web page.
  - Reinforce the importance of using effective prompts for understanding and applying web technologies.

- **Encouragement:**
  - Practice creating and styling web pages using the HTML and CSS concepts learned today.
  - Use AI tools to explore more advanced web development concepts and refine your skills.

---
