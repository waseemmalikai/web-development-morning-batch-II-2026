# 🧱 **Chapter 6: CSS Display & Layout Basics – How Elements Behave on the Web**

---

## 🧠 What You’ll Learn

By the end of this chapter, you’ll be able to:

✅ Understand the difference between **block**, **inline**, and **inline-block** elements
✅ Change how elements behave using the `display` property
✅ Control visibility and space using `visibility` and `display: none`
✅ Understand **default browser display behavior**
✅ Create a **Navbar & Button Row** mini-project

---

## 🌍 1. The Story: “Boxes with Personalities”

Imagine each HTML element has a *personality* —
some love to **take up the entire row** (block elements),
while others are **small and polite**, sharing space with others (inline elements).

These personalities decide how your page flows — and CSS gives you the power to **change those behaviors** anytime.

---

## 🧩 2. The `display` Property – The Boss of Layouts

The `display` property controls **how** an element behaves in the layout —
whether it sits alone, wraps text, or acts invisible.

---

## 🎯 Common Display Types

Let’s explore the most important ones first.

---

### 🧱 1️⃣ `display: block`

A **block-level** element always starts on a **new line**
and takes up the **full width** available.

Examples of default block elements:

* `<div>`
* `<p>`
* `<h1>` to `<h6>`
* `<section>`, `<header>`, `<footer>`

```css
div {
  display: block;
}
```

💡 Even if you don’t set it — these elements are block by default.

They:

* Respect width and height
* Push following elements to a new line
* Can have padding, margin, and borders

---

### 🧩 2️⃣ `display: inline`

**Inline elements** sit **side by side** on the same line,
and only take as much width as their content.

Examples:

* `<span>`
* `<a>`
* `<strong>`
* `<em>`

```css
span {
  display: inline;
}
```

💡 Inline elements:

* Ignore width and height
* Work well for styling **text inside lines**
* You can apply padding and margin horizontally, but not vertically (it won’t push neighbors up or down)

---

### 🧱 3️⃣ `display: inline-block`

This one’s the **best of both worlds** 😎
It behaves like **inline** (sits in a line)
but also allows **width, height, margin, and padding** like a block.

```css
button {
  display: inline-block;
  width: 120px;
  height: 40px;
}
```

Perfect for:

* Buttons
* Menu links
* Cards in a row

---

### 🧱 4️⃣ `display: none`

This **completely removes** an element from the layout —
it’s as if it doesn’t exist in the DOM visually.

```css
div {
  display: none;
}
```

💡 Use this to hide modals, menus, etc. (we’ll use it a lot later!)

---

### 🧩 5️⃣ `visibility: hidden`

This hides the element visually but still **reserves the space**.

```css
div {
  visibility: hidden;
}
```

Difference from `display: none`:

| Property             | Hidden from view | Space taken |
| -------------------- | ---------------- | ----------- |
| `display: none`      | ✅ Yes            | ❌ No        |
| `visibility: hidden` | ✅ Yes            | ✅ Yes       |

---

## 🧮 3. Default Display Behaviors (Browser Defaults)

Each HTML element has a **default display type**.

Example:

| Element                | Default Display |
| ---------------------- | --------------- |
| `<div>`, `<p>`, `<h1>` | block           |
| `<span>`, `<a>`, `<b>` | inline          |
| `<img>`                | inline-block    |
| `<table>`              | table           |
| `<li>`                 | list-item       |

💡 You can override any of these with `display`.

---

## 🧠 4. Example: Inline vs Block vs Inline-Block

Try this example 👇

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Display Example</title>
  <style>
    div {
      background: lightcoral;
      margin: 10px;
      padding: 10px;
      color: white;
    }

    span {
      background: lightgreen;
      padding: 10px;
      margin: 10px;
    }

    .block {
      display: block;
    }

    .inline {
      display: inline;
    }

    .inline-block {
      display: inline-block;
    }
  </style>
</head>
<body>
  <h2>Display Types</h2>
  <div class="block">Block Element</div>
  <div class="inline">Inline Element</div>
  <div class="inline-block">Inline-Block Element</div>
</body>
</html>
```

💥 Observe how each behaves differently!

---

## 🧰 5. Common Use Cases

| Task                 | Recommended Display |
| -------------------- | ------------------- |
| Paragraphs, sections | `block`             |
| Buttons side by side | `inline-block`      |
| Hide temporarily     | `display: none`     |
| Links in text        | `inline`            |

---

## 🧱 6. Mini Project: Navigation Bar & Button Row

Let’s use `display` to design a **simple responsive navbar** with inline-block buttons.

---

### 🧩 HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Navbar Project</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <nav class="navbar">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Services</a>
    <a href="#">Contact</a>
  </nav>
</body>
</html>
```

---

### 🧩 CSS

```css
body {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  background: #f4f6f8;
}

.navbar {
  background: #0072ff;
  padding: 15px;
  text-align: center;
}

.navbar a {
  display: inline-block;
  color: white;
  text-decoration: none;
  margin: 0 15px;
  padding: 10px 20px;
  border-radius: 5px;
  transition: 0.3s;
}

.navbar a:hover {
  background: rgba(255,255,255,0.2);
}
```

💡 Notice how `inline-block` allows us to control both spacing and shape for each link — perfect for navigation menus!

---

## 💎 7. Bonus: Toggle Visibility Example

You can easily show/hide elements dynamically (which we’ll later control via JavaScript).

```css
.hidden {
  display: none;
}
```

```html
<p class="hidden">This text is hidden!</p>
```

Later we’ll toggle this class to show/hide modals, menus, etc.

---

## 🧠 8. Recap

✅ `display` controls how elements behave in layout
✅ `block`, `inline`, `inline-block` are the most common
✅ `display: none` removes the element, `visibility: hidden` keeps space
✅ Default display types vary per element
✅ Built a real **Navbar Project**

---

## 🧩 Quick Quiz

1️⃣ What’s the main difference between `block` and `inline` elements?

2️⃣ Can you set width and height on inline elements?

3️⃣ Which property hides an element but keeps its space?

4️⃣ Which display type allows side-by-side boxes with custom width and height?



