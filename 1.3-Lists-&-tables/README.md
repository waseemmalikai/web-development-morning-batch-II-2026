# 🌍 Chapter 1.3 — HTML Lists & Tables

### 📖 Introduction

Lists and tables help organize information on a webpage.

* **Lists** → good for items, steps, or menus.
* **Tables** → good for structured data, like schedules, prices, or stats.

Learning lists and tables is important because most websites **display organized content** using these elements.

---

### 💡 Real-life Analogy

* **Lists** = shopping lists, to-do lists → easy to read.
* **Tables** = spreadsheets or restaurant menus → rows and columns organize information clearly.

---

### 🛠 Step-by-step Explanation

#### 1. HTML Lists

##### a) Unordered List (`<ul>` → bullets)

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

* `<ul>` → starts a bullet list.
* `<li>` → each list item.
* Bullets are default; can be styled with CSS later.

##### b) Ordered List (`<ol>` → numbers)

```html
<ol>
    <li>Wake up</li>
    <li>Brush teeth</li>
    <li>Have breakfast</li>
</ol>
```

* `<ol>` → starts a numbered list.
* `<li>` → each item.
* Can also be **alphabetical or Roman numerals** using `type` attribute:

```html
<ol type="A">
    <li>Option 1</li>
    <li>Option 2</li>
</ol>
```

##### c) Nested Lists

```html
<ul>
    <li>Fruits
        <ul>
            <li>Apple</li>
            <li>Banana</li>
        </ul>
    </li>
    <li>Vegetables
        <ul>
            <li>Carrot</li>
            <li>Spinach</li>
        </ul>
    </li>
</ul>
```

> Tip: Nested lists help organize sub-items.

---

#### 2. HTML Tables

##### a) Basic Table Structure

```html
<table border="1">
    <tr>
        <th>Name</th>
        <th>Age</th>
        <th>City</th>
    </tr>
    <tr>
        <td>Ali</td>
        <td>25</td>
        <td>Lahore</td>
    </tr>
    <tr>
        <td>Ayesha</td>
        <td>22</td>
        <td>Karachi</td>
    </tr>
</table>
```

**Explanation:**

* `<table>` → starts the table.
* `<tr>` → table row.
* `<th>` → table header (bold and centered).
* `<td>` → table data (normal cell).
* `border="1"` → adds simple border for visibility (we can style with CSS later).

---

##### b) Table Sections (`thead`, `tbody`, `tfoot`)

```html
<table border="1">
    <thead>
        <tr>
            <th>Product</th>
            <th>Price</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Laptop</td>
            <td>$500</td>
        </tr>
        <tr>
            <td>Mouse</td>
            <td>$20</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Total</td>
            <td>$520</td>
        </tr>
    </tfoot>
</table>
```

* `<thead>` → header row(s).
* `<tbody>` → main content rows.
* `<tfoot>` → footer row(s).

> Tip: Using sections makes tables **readable and easier to style with CSS**.

---

### 👨‍💻 Practical Demo

1. Open `index.html` in VS Code.
2. Add a list and table:

```html
<h2>My Hobbies</h2>
<ul>
    <li>Reading</li>
    <li>Cooking</li>
    <li>Programming</li>
</ul>

<h2>Student Info</h2>
<table border="1">
    <tr>
        <th>Name</th>
        <th>Grade</th>
    </tr>
    <tr>
        <td>Ali</td>
        <td>A+</td>
    </tr>
    <tr>
        <td>Ayesha</td>
        <td>A</td>
    </tr>
</table>
```

3. Save → Open with **Live Server** → see organized lists and tables in browser.

---

### 🎯 Learning Outcomes

By the end of this lecture, you will:

* Create **unordered and ordered lists**.
* Nest lists for **sub-items**.
* Create **basic tables** with headers and rows.
* Use `<thead>`, `<tbody>`, and `<tfoot>` for structured tables.
* Understand when to use **lists vs tables**.

