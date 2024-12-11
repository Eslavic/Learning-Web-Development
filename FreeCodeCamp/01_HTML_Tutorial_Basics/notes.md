# Project Notes: HTML Basics

---

## Why name the file `index.html`?

- Web servers automatically look for a file named `index.html` as the default entry point for a website.
- Naming it this way ensures compatibility and easy loading when someone accesses your project.

---

## **Key HTML Elements**

### **Basic Structure**

- **`<!DOCTYPE html>`**: Declares the document type as HTML5, all HTML files have to start with this **tag**.
- **`<html>`**: Root element of the HTML document.
- **`<body>`**: Contains all the visible content of the webpage.
- **`<head>`**: Contains metadata, styles, and links to external resources.

### **Common Tags**

- **Headings (`<h1>` to `<h6>`)**:
  - Define the hierarchy of titles and subtitles on a page.
  - `<h1>` is the main title, while `<h6>` is the smallest subheading.
- **Paragraph (`<p>`)**:
  - Used to add blocks of text content.
- **Image (`<img>`)**:
  - Displays images on the webpage. You can add [**attributes**](#html-attributes) to some **tags**.

### Semantic Elements

- **Semantic elements** describe the purpose of the content, improving readability for humans and search engines.

  - **`<main>`**: Wraps the main content of the page.

---

## **HTML Attributes**

- **Attributes** are properties or settings applied to HTML tags to modify their behavior or appearance. They are written inside the opening tag and follow the format:
  **`attribute="value"`**

### **Examples of some Common Attributes:**

- **`href`**: Specifies the URL for links.
- **`src`**: Specifies the source of the image.
- **`alt`**: Provides alternative text for images when they cannot be displayed.
- **`width`** & **`height`**: Define the size of the element in pixels or percentages.

### Example Code

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>HTML Project Freecodecamp</h1>
    <h2>My beautiful Dogs</h2>
    <main>
      <h3>Photoshot Esquitx</h3>
      <p>Click here to view Esquitx pictures</p>
      <img
        src="Gentleman_Esquitx.jpg"
        width="300"
        height="500"
        alt="A cute brown and orange dog sitting with a blue scarf"
      />
      <h3>Photoshot Stormy</h3>
      <p>Click here to view Stormy pictures</p>
      <!-- This is not gonna appear in the final output-->
      <img
        src="Stormy_Abrigado.jpg"
        width="300"
        height="500"
        alt="A cute Border Collie wearing a sweater, sitting next to a panda stuffed animal"
      />
    </main>
  </body>
</html>
```
