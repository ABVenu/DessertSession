### Student Notes

# Create and Deploy Your Website Using AI

---

### **1. Introduction**

- **What is a personal website?**
  - A personal website can showcase your skills, portfolio, and resume in a digital format.
  - It is useful for sharing your work with potential employers, clients, or collaborators.
- **Session Goal:**
  - You will learn how to structure, style, and publish your own resume or portfolio as a single-page website.

---

### **2. Recap of HTML and CSS Basics**

- **HTML Tags to Remember:**

  - `div`: Used to structure the layout of the webpage.
  - `h1`, `h2`, `h3`: Headings for sections (e.g., your name, profession).
  - `p`: Paragraphs for text (e.g., your bio, skills description).
  - `img`: For adding images (e.g., your profile photo).
  - `a`: Links to other websites or sections.
  - `input`: Fields for forms (e.g., for contact information).
  - `button`: Buttons for actions like submitting a form.

- **Basic CSS Properties:**
  - `background-color`: Adds background color to elements.
  - `font-size`: Changes the size of text.
  - `padding`: Adds space inside the border of elements.
  - `margin`: Adds space outside the element.
  - `text-align`: Aligns text (e.g., center, left, right).

---

### **3. Introduction to Flexbox**

- **What is Flexbox?**
  - Flexbox is a CSS layout model that makes it easy to align elements on a webpage.
- **Key Flexbox Properties:**

  - `display: flex`: Defines a flex container that arranges items inside it.
  - `flex-direction`: Controls the direction of the layout (row or column).
  - `justify-content`: Aligns items along the main axis (e.g., center, space-between).
  - `align-items`: Aligns items along the cross-axis (e.g., center, flex-start).

- **Why use Flexbox?**
  - It simplifies the process of building flexible, responsive layouts without needing to adjust individual margins or paddings for each element.

---

### **4. Building Your Website Structure**

- **Essential Sections for Your Website:**

  1. **Header**: Your name, profession, and simple navigation links.
  2. **About Me**: A brief bio or introduction about who you are.
  3. **Skills/Projects**: A list of skills you possess or projects you’ve worked on.
  4. **Contact**: A form where visitors can contact you or links to your social media profiles.

- **HTML Structure Example:**

```html
<div class="header">
  <h1>Your Name</h1>
  <p>Profession (e.g., Web Developer)</p>
</div>

<div class="about">
  <h2>About Me</h2>
  <p>A short bio about yourself.</p>
</div>

<div class="skills">
  <h2>Skills</h2>
  <ul>
    <li>Skill 1</li>
    <li>Skill 2</li>
    <li>Skill 3</li>
  </ul>
</div>

<div class="contact">
  <h2>Contact</h2>
  <form>
    <input type="text" placeholder="Your Name" />
    <input type="email" placeholder="Your Email" />
    <button>Submit</button>
  </form>
</div>
```

---

### **5. Styling the Website with CSS**

- **Key CSS Properties to Apply:**

  - Use `padding` and `margin` to give space around your elements.
  - Use Flexbox to align sections vertically or horizontally for a clean layout.

- **CSS Example:**

```css
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
}

.header {
  text-align: center;
  background-color: #333;
  color: #fff;
  padding: 20px;
}

.about,
.skills,
.contact {
  padding: 20px;
  margin: 20px auto;
  max-width: 800px;
}

form {
  display: flex;
  flex-direction: column;
}

button:hover {
  background-color: #555;
}
```

- **Tips for Flexbox:**
  - To center elements within a section, use `justify-content: center` and `align-items: center` on the flex container.
  - To create horizontal navigation, use `flex-direction: row`.

---

### **6. Deploying Your Website Using Netlify**

- **What is Netlify?**
  - Netlify is a platform that allows you to deploy your website online for free.
- **Steps to Deploy:**
  1. Go to [Netlify](https://www.netlify.com/) and create a free account.
  2. Once signed in, go to **Sites** and click **Add New Site**.
  3. Select **Deploy manually** by dragging your HTML and CSS files into the upload area.
  4. Netlify will automatically deploy your website and give you a live URL.
- **After Deployment:**
  - You can share the URL with others.
  - If you make changes to your website, you can re-upload the updated files to Netlify.

---

### **Assignment**

1. **Flexbox Practice:**

   - Create a webpage with two sections: an image gallery and a contact form, using Flexbox for layout.

2. **Website Enhancements:**
   - Continue refining and adding more styles and content to your portfolio website, based on what you've learned.

---

### **Summary**

- Today, you learned how to create and style a single-page website using HTML, CSS, and Flexbox.
- You also deployed your website using Netlify, making it live for others to visit.

Remember to keep practicing with Flexbox and CSS to improve your web design skills! You can always update your portfolio as you learn more and showcase it to future employers.
