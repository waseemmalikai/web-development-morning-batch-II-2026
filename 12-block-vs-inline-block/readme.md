# 📏 **Chapter 16 – Inline vs Block Elements**

### 📖 Introduction

One of the **biggest confusions for beginners** is why some elements start on a **new line** (like `<p>` or `<div>`), while others stay **inline with text** (like `<span>` or `<a>`).

This difference is called **display behavior**:

* **Block-level elements** → take full width, always start on a new line.
* **Inline elements** → only take as much space as needed, flow with text.

Understanding this is crucial before moving into **CSS (layouts, Flexbox, Grid)**.

---

### 💡 Real-Life Analogy

Imagine you’re arranging furniture:

* A **sofa** (block element) → takes the whole width of the room.
* A **chair** (inline element) → sits neatly beside other chairs in the same line.

Both are furniture, but they behave differently in space.

---

### 🛠 Step-by-Step Explanation

#### 1. Block Elements

* Always start on a **new line**.
* Take full available width.
* Can contain other block & inline elements.

Examples: `<div>`, `<p>`, `<h1>–<h6>`, `<section>`, `<article>`.

```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

📌 Each paragraph starts on a **new line**.

---

#### 2. Inline Elements

* Do **not start** on a new line.
* Take only as much width as content.
* Usually used for formatting text.

Examples: `<span>`, `<a>`, `<strong>`, `<em>`, `<img>`.

```html
<p>This is <strong>bold</strong> text inside a paragraph.</p>
```

📌 The `<strong>` element stays **inline**, doesn’t break the flow.

---

#### 3. Comparing Block vs Inline

```html
<div style="border: 2px solid red;">Block Element</div>
<span style="border: 2px solid blue;">Inline Element</span>
<span style="border: 2px solid green;">Another Inline</span>
```

🖼️ Output:

* Red box spans across the full line.
* Blue & green boxes sit next to each other in the same line.

---

#### 4. Inline-Block (Bonus)

* Behaves like inline (sits in line), but allows **block properties** (width, height, margin).

```html
<span style="display:inline-block; width:100px; height:50px; background:yellow;">Inline-Block</span>
```
