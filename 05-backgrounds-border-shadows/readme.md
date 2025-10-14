# 🎨 **Chapter 5: Backgrounds, Borders & Shadows – Styling Like a Pro**

---

## 🧠 What You’ll Learn

By the end of this chapter, you’ll be able to:

✅ Add background colors, images, and gradients
✅ Control how images repeat, position, and size
✅ Design creative borders with radius and images
✅ Add stunning shadows for depth (box & text shadows)
✅ Create a beautiful **"Business Card" project**

---

## 🌍 1. The Story: “Turning Plain Boxes into Beautiful Cards”

In the last chapter, we built simple boxes — clean but flat.
Now imagine you’re a designer decorating your **first digital business card** —
adding colors, gradients, a photo background, and a soft glow beneath.

That’s what **CSS backgrounds, borders, and shadows** allow you to do.
They make plain content look **alive**.

---

## 🎨 2. Backgrounds – Coloring & Decorating Elements

The `background` property lets you control how an element’s background looks.

---

### 🎯 1️⃣ Background Color

The simplest one:

```css
div {
  background-color: lightblue;
}
```

💡 You can use:

* Color names: `red`, `green`, `blue`
* HEX codes: `#4CAF50`
* RGB: `rgb(255, 0, 0)`
* RGBA: `rgba(0, 0, 0, 0.5)` → adds transparency
* HSL: `hsl(120, 50%, 50%)`

---

### 🎯 2️⃣ Background Image

You can set any image behind an element:

```css
div {
  background-image: url('image.jpg');
}
```

---

### 🎯 3️⃣ Controlling Image Behavior

| Property                | Description       | Example                             |
| ----------------------- | ----------------- | ----------------------------------- |
| `background-repeat`     | Repeat or not     | `no-repeat`, `repeat-x`, `repeat-y` |
| `background-position`   | Where to place it | `center`, `top right`, `10px 20px`  |
| `background-size`       | Scale the image   | `cover`, `contain`, `100% 100%`     |
| `background-attachment` | Scroll or fixed   | `fixed`, `scroll`                   |

Example:

```css
div {
  background-image: url('bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
```

💡 `cover` = fills the area while maintaining aspect ratio
💡 `contain` = fits the image completely inside the box

---

### 🎯 4️⃣ Background Gradient (No Image Needed!)

You can create smooth color blends using gradients.

**Linear Gradient:**

```css
div {
  background: linear-gradient(to right, #00c6ff, #0072ff);
}
```

**Radial Gradient:**

```css
div {
  background: radial-gradient(circle, #ff9a9e, #fad0c4);
}
```

💡 You can add as many color stops as you want.

---

### 🎯 5️⃣ Background Shorthand

Instead of writing many lines:

```css
div {
  background: url('bg.jpg') no-repeat center/cover #f4f4f4;
}
```

---

## 🧱 3. Borders – Outlining Your Elements

Borders define the **edges** of your elements.

---

### 🎯 1️⃣ Basic Border

```css
div {
  border: 3px solid #4CAF50;
}
```

---

### 🎯 2️⃣ Border Styles

| Style                                | Example         |
| ------------------------------------ | --------------- |
| `solid`                              | Continuous line |
| `dashed`                             | Short dashes    |
| `dotted`                             | Dotted line     |
| `double`                             | Two lines       |
| `groove`, `ridge`, `inset`, `outset` | 3D effects      |

---

### 🎯 3️⃣ Border Radius (Rounded Corners)

```css
div {
  border-radius: 10px;
}
```

💡 You can make:

* Circles: `border-radius: 50%;`
* Ovals: `border-radius: 50px / 25px;`
* One-sided curves: `border-top-left-radius: 20px;`

---

### 🎯 4️⃣ Border Image (Advanced)

You can use an image as a border:

```css
div {
  border: 10px solid transparent;
  border-image: url('border.png') 30 round;
}
```

---

## 🌫️ 4. Shadows – Adding Depth and Realism

Shadows make your elements feel **3D** and alive.

---

### 🎯 1️⃣ Box Shadow

```css
div {
  box-shadow: 5px 5px 15px rgba(0,0,0,0.3);
}
```

📘 Syntax:

```
box-shadow: x-offset y-offset blur spread color;
```

Example:

```css
box-shadow: 0 4px 10px rgba(0,0,0,0.2);
```

💡 You can even make **inner shadows**:

```css
box-shadow: inset 0 4px 10px rgba(0,0,0,0.2);
```

---

### 🎯 2️⃣ Multiple Shadows

```css
div {
  box-shadow:
    0 4px 10px rgba(0,0,0,0.2),
    0 0 20px rgba(0,255,0,0.3);
}
```

---

### 🎯 3️⃣ Text Shadow

```css
h1 {
  text-shadow: 2px 2px 5px rgba(0,0,0,0.4);
}
```

💡 Great for glowing titles or embossed effects.

---

## 💎 5. Real-Life Mini Project – Business Card

Let’s apply everything: backgrounds, borders, and shadows.

---

### 🧩 HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Business Card</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="card">
    <img src="https://via.placeholder.com/100" alt="Profile">
    <h2>Ali Raza</h2>
    <p>UI/UX Designer</p>
    <button>Hire Me</button>
  </div>
</body>
</html>
```

---

### 🧩 CSS

```css
body {
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(to right, #00c6ff, #0072ff);
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.card {
  background: white;
  border-radius: 15px;
  padding: 25px;
  text-align: center;
  width: 300px;
  box-shadow: 0 6px 20px rgba(0,0,0,0.15);
  border: 2px solid #f0f0f0;
}

.card img {
  border-radius: 50%;
  border: 4px solid #0072ff;
  margin-bottom: 15px;
}

.card h2 {
  margin: 10px 0 5px;
}

.card p {
  color: #777;
  margin-bottom: 20px;
}

.card button {
  background: #0072ff;
  color: white;
  border: none;
  padding: 10px 25px;
  border-radius: 8px;
  cursor: pointer;
  transition: 0.3s;
}

.card button:hover {
  box-shadow: 0 5px 15px rgba(0,114,255,0.4);
  background: #005fd1;
}
```

💥 Congratulations — you just built your first **beautiful, modern business card** using pure CSS!

---

## 🧠 6. Recap

✅ `background` controls colors, images, and gradients
✅ `border` adds edges and shapes (solid, dashed, radius, image)
✅ `box-shadow` & `text-shadow` add depth and glow
✅ Used all of them to create a professional **Business Card** design

---

## 🧩 Quick Quiz

1️⃣ What’s the difference between `cover` and `contain` in background-size?
2️⃣ How do you create rounded corners?
3️⃣ What’s the syntax for `box-shadow`?
4️⃣ Can you use multiple shadows in one element?

