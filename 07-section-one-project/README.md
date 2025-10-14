# 🎯 **Mini Projects — Section 1 (CSS Foundations)**

---

## 🧩 **Project 1: Personal Bio Card Design**

### 🎓 Goal

Design a **Personal Bio Card** that displays your name, photo, profession, and short description — applying everything you learned:

* Colors 🎨
* Fonts & Typography 🖋️
* Padding / Margin / Border (Box Model)
* Display types & alignment

---

### 🧱 Step 1 – HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Personal Bio Card</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="bio-card">
    <img src="https://via.placeholder.com/120" alt="Profile Photo">
    <h2>Sarah Ahmed</h2>
    <h4>Frontend Developer</h4>
    <p>
      Passionate about crafting beautiful web experiences with 
      HTML, CSS, and JavaScript. Loves minimal design and clean code.
    </p>
    <button>Contact Me</button>
  </div>
</body>
</html>
```

---

### 🎨 Step 2 – CSS Styling

```css
body {
  background: #f0f4f8;
  font-family: 'Poppins', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.bio-card {
  background: #fff;
  padding: 25px;
  width: 280px;
  text-align: center;
  border-radius: 15px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.bio-card img {
  border-radius: 50%;
  border: 4px solid #007bff;
  margin-bottom: 15px;
}

.bio-card h2 {
  color: #333;
  margin: 10px 0 5px;
}

.bio-card h4 {
  color: #007bff;
  margin-bottom: 15px;
  font-weight: 500;
}

.bio-card p {
  color: #555;
  font-size: 14px;
  margin-bottom: 20px;
  line-height: 1.5;
}

.bio-card button {
  display: inline-block;
  background: #007bff;
  color: #fff;
  border: none;
  padding: 10px 20px;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.3s;
}

.bio-card button:hover {
  background: #0056b3;
}
```

---

### ✨ Concepts Applied

| Concept       | Usage                            |
| ------------- | -------------------------------- |
| Colors        | Background + button themes       |
| Fonts         | Imported Google Font (`Poppins`) |
| Box Model     | Padding, margin, border, shadow  |
| Display       | Centered with Flexbox            |
| Border Radius | Circular photo + rounded card    |
| Transitions   | Smooth hover effect on button    |

---

### ✅ Output Preview

A white, rounded card centered on a light background with:

* Circular photo
* Name & job title
* Small bio paragraph
* Stylish “Contact Me” button

---

## 🧩 **Project 2: Simple Product Card**

### 🎯 Goal

Create a **Product Card** layout that demonstrates:

* `display: inline-block` vs `block`
* Borders, padding, and shadows
* Font and color hierarchy

---

### 🧱 Step 1 – HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Product Card</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="product-card">
    <img src="https://via.placeholder.com/250x180" alt="Product">
    <h3>Wireless Headphones</h3>
    <p>High-quality sound, Bluetooth 5.0, 24 h battery life.</p>
    <span class="price">$59.99</span>
    <button>Add to Cart</button>
  </div>
</body>
</html>
```

---

### 🎨 Step 2 – CSS Styling

```css
body {
  background: #f7f7f7;
  font-family: 'Poppins', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.product-card {
  background: #fff;
  display: inline-block;
  width: 260px;
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 15px;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
}

.product-card img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 10px;
}

.product-card h3 {
  color: #222;
  font-size: 18px;
  margin: 10px 0;
}

.product-card p {
  color: #555;
  font-size: 14px;
  margin-bottom: 10px;
}

.product-card .price {
  display: block;
  font-size: 16px;
  font-weight: 600;
  color: #28a745;
  margin-bottom: 12px;
}

.product-card button {
  background: #007bff;
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: 6px;
  cursor: pointer;
  transition: 0.3s;
}

.product-card button:hover {
  background: #0056b3;
}
```

---

### ✨ Concepts Applied

| Concept           | Usage                             |
| ----------------- | --------------------------------- |
| Display types     | `inline-block` for layout control |
| Box Model         | Padding, border, margin           |
| Colors            | Background, price highlight       |
| Fonts & Hierarchy | Heading > description > price     |
| Shadows + radius  | Card depth and soft corners       |

---

### ✅ Output Preview

A clean product card with:

* Product image
* Name, description, price
* Rounded edges and shadow
* “Add to Cart” button with hover effect

---

## 🧠 **What Students Learn Here**

By finishing these two mini projects, students will:

* Understand how **every CSS property works together**
* Gain confidence designing small, real-world components
* Be ready to move on to **CSS Positioning & Layout Systems** (next section)
