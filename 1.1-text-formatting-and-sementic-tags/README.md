# 🌍 Chapter 1.1 — HTML Text Formatting & Semantic Tags

### 📖 Introduction

Text is the most common content on web pages. HTML gives us **special tags** to format text, like **bold, italic, or underlined**, and to **give meaning** to sections using **semantic tags**.

Semantic tags help browsers and search engines **understand what your content means**, not just how it looks. This is important for **SEO**, **accessibility**, and maintaining **clean code**.

---

### 💡 Real-life Analogy

* Formatting tags are like **highlighters, pens, and markers** for your text → they make important words stand out.
* Semantic tags are like **labels on boxes** → they tell everyone (humans and machines) what is inside.

---

### 🛠 Step-by-step Explanation

#### 1. Text Formatting Tags

| Tag        | Effect / Use                           |
| ---------- | -------------------------------------- |
| `<b>`      | Bold text (visual only)                |
| `<strong>` | Bold and **important** semantically    |
| `<i>`      | Italic text (visual only)              |
| `<em>`     | Italic and **emphasized** semantically |
| `<u>`      | Underline text                         |
| `<mark>`   | Highlighted text                       |
| `<small>`  | Smaller text                           |
| `<del>`    | Strikethrough / deleted text           |
| `<ins>`    | Inserted text (underline usually)      |
| `<sub>`    | Subscript (like H₂O)                   |
| `<sup>`    | Superscript (like x²)                  |

**Example:**

```html
<p>This is <b>bold</b> text.</p>
<p>This is <strong>strong</strong> text.</p>
<p>This is <i>italic</i> text.</p>
<p>This is <em>emphasized</em> text.</p>
<p>This is <u>underlined</u> text.</p>
<p>This is <mark>highlighted</mark> text.</p>
<p>H<sub>2</sub>O is water.</p>
<p>x<sup>2</sup> = x squared.</p>
```

> Tip: Use `<strong>` and `<em>` for meaning, not just style. This is better for SEO and accessibility.

---

#### 2. Line Breaks and Horizontal Rules

* `<br>` → Forces a **line break** (like pressing Enter).
* `<hr>` → Adds a **horizontal line** to separate sections.

Example:

```html
<p>Hello!<br>Welcome to HTML.</p>
<hr>
<p>New section starts here.</p>
```

---

#### 3. Semantic HTML Tags

Semantic tags **describe the role of content**:

| Tag            | Use                             |
| -------------- | ------------------------------- |
| `<header>`     | Header of a page or section     |
| `<nav>`        | Navigation menu                 |
| `<main>`       | Main content of the page        |
| `<section>`    | Section of content with a theme |
| `<article>`    | Independent article or post     |
| `<aside>`      | Sidebar or extra info           |
| `<footer>`     | Footer of page or section       |
| `<figure>`     | Image or illustration           |
| `<figcaption>` | Caption for figure/image        |

**Example Structure:**

```html
<body>
  <header>
    <h1>My Website</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">About</a>
    </nav>
  </header>

  <main>
    <section>
      <h2>Introduction</h2>
      <p>This is the first section of content.</p>
    </section>

    <article>
      <h3>Blog Post</h3>
      <p>This is a sample article.</p>
    </article>

    <aside>
      <p>Extra info or links.</p>
    </aside>
  </main>

  <footer>
    <p>&copy; 2026 My Website</p>
  </footer>
</body>
```

> Semantic tags make your HTML **structured, readable, and SEO-friendly**.

---

#### 4. Why Semantic HTML is Important

* **Accessibility:** Screen readers for visually impaired users can understand your content.
* **SEO:** Search engines like Google understand your content better.
* **Maintainability:** Easier for you and others to read and edit code.

---

### 👨‍💻 Practical Demo

1. Open `index.html` in VS Code.
2. Add a semantic structure with headings, paragraphs, and a footer.
3. Format text using `<strong>`, `<em>`, `<mark>`, and `<sub>/<sup>`.
4. Open in **Live Server** → see how everything looks structured and readable.

```html
<header>
    <h1>HTML Mastery Course</h1>
</header>
<main>
    <section>
        <h2>Lesson 1: Text Formatting</h2>
        <p>Use <strong>bold</strong> and <em>italic</em> wisely.</p>
    </section>
</main>
<footer>
    <p>&copy; 2026 Waseem Malik</p>
</footer>
```

---

### 🎯 Learning Outcomes

By the end of this lecture, you will:

* Use **text formatting tags** to style your content.
* Understand and implement **semantic HTML tags**.
* Create **structured, readable, and accessible webpages**.
* Know why semantic HTML is important for **SEO and accessibility**.