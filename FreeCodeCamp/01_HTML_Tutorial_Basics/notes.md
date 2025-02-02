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
- **Anchor Element (`<a>`)**:
  - The `<a>` element creates a hyperlink, allowing users to navigate to another webpage, a specific section within the same page, or even trigger downloads.
  - It requires the [**href**](#examples-of-some-common-attributes) attribute.
- **List Elements (`<ul>, <ol>`)**:
  - **Unordered List (`<ul>`)**: Creates an unordered list (bulleted list).
  - **Ordered List (`<ol>`)**: Creates an ordered (numbered) list.
  - **List Item (`<li>`)**: Represents an item in either type of list (`<ul>` or `<ol>`).
- **Text Emphasis Elements(`<strong>, <em>`)**:
  - **`<strong>`**: Makes text <strong>bold</strong> and gives it semantic importance.
  - **`<em>`**: Emphasizes text by displaying it in <em>italics</em>.
- **Form and Input Elements(`<form>, <input>, <button>`)**:
  - **`<form> `**: Used to create interactive forms that allow users to submit data.
  - **`<input>`**: Used to collect user input. It can have different types depending on what kind of input you need.
  - **`<button>`**: Creates a clickable button. It is often used inside forms to submit data.

### Semantic Elements

- **Semantic elements** describe the purpose of the content, improving readability for humans and search engines.

  - **`<main>`**: Wraps the main content of the page.

---

## **HTML Attributes**

- **Attributes** are properties or settings applied to HTML tags to modify their behavior or appearance. They are written inside the opening tag and follow the format:
  **`attribute="value"`**

### **Examples of some Common Attributes:**

- **`src`**: Specifies the source of the image (used in the `<img>` tag).
- **`href`**: Specifies the URL or destination of the link (used in the `<a>` tag).
  <details>
    <summary>Click for more <strong><code>href</code></strong> variations</summary>
    <ul>
      <li><code>href="link"</code>: Most commonly used.</li>
      <li><code>href="#"</code>: Creates a placeholder link that doesn’t lead anywhere.</li>
    </ul>
  </details>
- **`alt`**: Provides alternative text for images when they cannot be displayed.
- **`width`** & **`height`**: Define the size of the element in pixels or percentages (commonly used in images and other media).
- **`target="_blank`**: Opens the linked page in a new tab or window (used in the `<a>` tag).

### Example Code

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Adventures of Esquitx and Stormy</h1>
    <h2>Who is Esquitx and Stormy?</h2>
    <p>
      Esquitx and Stormy are two incredible dogs who have brought endless joy to
      my life. Their personalities are as different as night and day, and they
      never fail to keep me on my toes.
    </p>
    <main>
      <h3>Photoshot Esquitx</h3>
      <p>Click here to view Esquitx pictures</p>
      <img
        src="Assets/Gentleman_Esquitx.jpg"
        width="300"
        height="500"
        alt="A cute brown and orange dog sitting with a blue scarf"
      />
      <h4>Things Esquitx love:</h4>
      <ul>
        <li>The beach</li>
        <li>Food, especially meat</li>
        <li>Run and walk in a sunny day</li>
        <li>Caresses between back and butt</li>
      </ul>
      <h3>Photoshot Stormy</h3>
      <p>
        <a href="#" target="_blank">Click here to view Stormy pictures</a>
      </p>
      <!-- This is not gonna appear in the final output-->
      <img
        src="Assets/Stormy_Abrigado.jpg"
        width="300"
        height="500"
        alt="A cute Border Collie wearing a sweater, sitting next to a panda stuffed animal"
      />
      <h4>Things Stormy love</h4>
    </main>
  </body>
</html>
```
