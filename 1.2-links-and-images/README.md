# 🌍 Chapter 1.2 — HTML Links & Images

### 📖 Introduction

Webpages are not isolated; they **connect to other pages** and often include **images** to make content attractive.

In this lesson, you will learn:

* How to **add links** to other pages or websites.
* How to **add images** to your webpage.
* How to use **attributes** like `href`, `src`, `alt`, and `target`.

---

### 💡 Real-life Analogy

* **Links** = roads or bridges → they connect one place to another.
* **Images** = posters, photos, or illustrations → make information easier to understand and visually appealing.

---

### 🛠 Step-by-step Explanation

#### 1. HTML Links

HTML uses the `<a>` tag (anchor) to create links.

**Basic Syntax:**

```html
<a href="https://www.google.com">Visit Google</a>
```

**Explanation:**

* `<a>` → opening anchor tag.
* `href="URL"` → the link address (Hypertext Reference).
* Text inside → visible clickable text.
* `</a>` → closing tag.

**Open link in new tab:**

```html
<a href="https://www.google.com" target="_blank">Google</a>
```

---

#### 2. Relative vs Absolute Links

* **Absolute link:** full URL → points to another website.

```html
<a href="https://www.example.com">External Site</a>
```

* **Relative link:** path to another file in your project → points to local page.

```html
<a href="about.html">About Page</a>
```

---

#### 3. HTML Images

HTML uses `<img>` tag to display images.

**Basic Syntax:**

```html
<img src="image.jpg" alt="My Image">
```

**Explanation:**

* `src="image.jpg"` → source path of the image.
* `alt="My Image"` → text displayed if image cannot load; also important for **accessibility**.
* `<img>` is **self-closing**, no `</img>` needed.

**Optional attributes:**

* `width` and `height` → control image size.
* `title` → tooltip on hover.

Example:

```html
<img src="flower.jpg" alt="Beautiful Flower" width="300" height="200" title="Flower Image">
```

---

#### 4. Linking Images

You can make images clickable by **wrapping them inside `<a>`**:

```html
<a href="https://www.google.com">
    <img src="logo.png" alt="Google Logo">
</a>
```

Clicking the image will now open the link.

---

#### 5. Best Practices

* Always use **alt text** for images → helps visually impaired users and improves SEO.
* Use **relative links** for local pages → makes moving projects easier.
* Keep **image file sizes small** → website loads faster.

---

### 👨‍💻 Practical Demo

1. Open `index.html` in VS Code.
2. Add links and images:

```html
<h1>My Favorite Sites</h1>
<p>Visit <a href="https://www.google.com" target="_blank">Google</a></p>
<p>Visit <a href="about.html">About Page</a></p>

<h2>My Favorite Images</h2>
<img src="flower.jpg" alt="Beautiful Flower" width="300">
<a href="https://www.wikipedia.org">
    <img src="wikipedia.png" alt="Wikipedia Logo" width="150">
</a>
```

3. Save → Open with **Live Server** → test links and images in browser.

---

### 🎯 Learning Outcomes

By the end of this lecture, you will:

* Add **links** to other pages and websites.
* Understand **relative vs absolute links**.
* Add **images** to your web page with proper `src` and `alt`.
* Make images **clickable links**.
* Follow **best practices** for links and images.
