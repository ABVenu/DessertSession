### Create Your Own Resume/Portfolio Website from Scratch using Gen AI

#### Submission Guidelines

- Please submit the deployed Link (using Netlify)
- Instructions to deploy:
    - Please code in the OneCompiler [Template Link](https://onecompiler.com/html/42rrx8jyu) and Download the file, keep the downloaded file in a any desired folder, ensure its name is index (if not, please rename it), 
    - Then open Netlify and Login, Then click on `Add New Site`, Then click on `Manual Deploy` Button and Select the folder, where the downloaded file is kept
    - Once you select the folder, then click on `Upload`, then you will get the `Deployed Link`

**Objective**: Build a personal resume or portfolio website that showcases your skills, projects, and contact information. This will be a single-page website created entirely by you, from structure to deployment. Additionally, you will incorporate basic JavaScript events to enhance the interactivity of your website.

---

### **Instructions:**

1. **Website Structure**:

   - Create a new HTML file and structure it as follows:
     - **Header**:
       - Your full name.
       - A brief tagline or profession (e.g., "Web Developer" or "Graphic Designer").
     - **About Section**:
       - A short paragraph introducing yourself.
       - Include a profile picture using the `img` tag.
       - Keep you picture in google drive and share it by keeping `Anyone` with the link, use this link as `src`
     - **Skills Section**:
       - List at least 5 skills (e.g., "HTML", "CSS", "Problem Solving").
     - **Projects Section**:
       - Add descriptions of 2 projects (real or fictional). Each project should include:
         - The project name.
         - A short description of what you did.
         - An optional link to a live demo or repository.
     - **Contact Section**:
       - Add a simple heading, and hide your contact details (email, phone) initially.
       - Provide a "Show Contact Info" button, and use JavaScript to reveal your contact details when clicked.

2. **Layout Design Using Flexbox**:

   - Use **Flexbox** to align and structure the following sections:
     - The **header** should be centered horizontally on the page.
     - In the **projects section**, display project details side by side using `flex-direction: row`.
     - For the **contact section**, center the form inputs and buttons on the page using Flexbox.

3. **Styling the Website with CSS**:

   - Add your own styles using CSS:
     - **Background Color**: Choose a background color that complements the content (e.g., light gray or white).
     - **Text Styles**: Set font sizes and colors for headings (`h1`, `h2`, `h3`) and paragraphs.
     - **Hover Effects**: Add hover effects to buttons and links, changing their background or text color when the user hovers over them.
     - **Padding and Margin**: Apply padding and margin to create space around elements for better readability.

4. **Incorporating JavaScript Events**:

   - Enhance your website's interactivity by adding the following simple events:

     - **Click Event to Show Contact Info**:

       - In the **contact section**, add a button labeled "Show Contact Info". When clicked, it should reveal your contact information (email, phone number) that was hidden by default.

     - **Mouseover Event to Highlight Skills**:
       - In the **skills section**, highlight a skill when the user hovers over it by changing its background color.

5. **Deployment**:
   - Once your website is complete, deploy it online using **Netlify**:
     - Sign in to Netlify and upload your HTML, CSS, and JavaScript files.
     - Once deployed, share the live URL of your portfolio website.

---
