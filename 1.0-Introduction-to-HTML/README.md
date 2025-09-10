# 🌍 Chapter 1.0 — Introduction to HTML

### 📖 Introduction

HTML stands for **HyperText Markup Language**.
It is the **language of the web** — every website you visit uses HTML.

HTML is **not a programming language**. Instead, it is a **markup language**. This means it tells the browser **how to structure content** on a webpage.

Think of HTML as the **skeleton of a webpage** — it creates the structure, while CSS adds style (colors, fonts) and JavaScript adds behavior (click buttons, animations).

---

### 💡 Real-life Analogy

Imagine building a **house**:

* **HTML** = bricks, walls, doors, and windows → structure of the house.
* **CSS** = paint, tiles, decorations → how the house looks.
* **JavaScript** = electricity, fans, sensors → makes the house interactive.

Without HTML, your webpage **won’t exist**.

---

### 🛠 Step-by-step Explanation

#### 1. Basic HTML Structure

Every HTML page follows a **basic structure**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Webpage</title>
</head>
<body>
    <h1>Welcome to HTML!</h1>
    <p>This is my first web page.</p>
</body>
</html>
```

**Explanation:**

* `<!DOCTYPE html>` → tells the browser that this is an HTML5 document.
* `<html>` → the root element, wraps all HTML content.
* `<head>` → contains metadata, title, links to CSS/JS.
* `<meta charset="UTF-8">` → ensures proper display of characters (like Urdu, Hindi, emojis).
* `<title>` → title shown on browser tab.
* `<body>` → contains all visible content like text, images, links.

---

#### 2. HTML Elements & Tags

HTML uses **tags** to define elements.

* A **tag** is like a container.
* Most tags have an **opening tag** `<tag>` and **closing tag** `</tag>`.

Example:

```html
<p>This is a paragraph.</p>
```

* `<p>` → opening tag.
* `</p>` → closing tag.
* Text inside = content of the element.

Some tags are **self-closing** (no closing tag needed):

```html
<img src="image.jpg" alt="My Image">
<br>
<hr>
```

---

#### 3. Common HTML Tags

| Tag           | Use                                        |
| ------------- | ------------------------------------------ |
| `<h1>`…`<h6>` | Headings (h1 = biggest, h6 = smallest)     |
| `<p>`         | Paragraphs                                 |
| `<a>`         | Links                                      |
| `<img>`       | Images                                     |
| `<ul>`        | Unordered list (bullets)                   |
| `<ol>`        | Ordered list (numbers)                     |
| `<li>`        | List item                                  |
| `<div>`       | Division / container for grouping elements |
| `<span>`      | Inline container for styling small text    |

---

#### 4. Nesting HTML Elements

You can put elements **inside other elements**:

```html
<div>
    <h2>My Skills</h2>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>
</div>
```

> Tip: Always close your tags properly to avoid errors.

---

#### 5. Comments in HTML

Comments are **notes for developers** and do **not show on the webpage**:

```html
<!-- This is a comment -->
<p>Hello World!</p>
```

---

### 👨‍💻 Practical Demo

1. Open VS Code → `index.html`.
2. Type the HTML boilerplate (`!` + Tab).
3. Add a heading and paragraph:

```html
<body>
    <h1>Learning HTML</h1>
    <p>HTML is easy and fun!</p>
</body>
```

4. Save → Open with Live Server → See your webpage in the browser.

---

### 🎯 Learning Outcomes

After this lecture you will:

* Understand **what HTML is** and why it is important.
* Know the **basic structure** of an HTML page.
* Use common tags like headings, paragraphs, lists, links, and images.
* Understand **nesting of elements** and proper tag closure.
* Add **comments** to your code.
