## 🌐 **Chapter 12 – The HTML `<head>` Section (Metadata & SEO Basics)**

### 📖 Introduction

When you open a webpage, you mostly see the **body content**: text, images, buttons. But did you know there’s a hidden section that browsers, search engines, and even social media rely on? That’s the **HTML `<head>` section**.

The `<head>` doesn’t display content directly to users but contains **metadata** (data about data) — instructions that tell browsers **how to render the page**, tell search engines **how to index it**, and tell social media **how to show previews**.

Without a proper `<head>`, your website might:

* Not display correctly on mobile phones.
* Look ugly when shared on Facebook or Twitter.
* Rank poorly in Google search results.

So this chapter is about **making your site professional, discoverable, and responsive**.

---

### 💡 Real-Life Analogy

Think of the `<head>` like a **resume header**:

* Your **name & title** = `<title>` of the page.
* Your **profile photo** = favicon.
* Your **summary** = `<meta description>`.
* Your **contact info** = metadata for sharing (Open Graph tags).

Just like HR may reject a resume with a missing header, search engines and browsers may “reject” or mishandle a site without a proper `<head>`.

---

### 🛠 Step-by-Step Explanation

#### 1. The `<title>` Tag

* Defines the **title of the page** shown in the browser tab.
* Important for **SEO & user bookmarks**.

```html
<head>
  <title>Future Programming - Learn HTML</title>
</head>
```

#### 2. `<meta charset>` (Character Encoding)

* Defines how characters (letters, emojis, symbols) are stored.
* Always use **UTF-8** → supports global languages, including Urdu, Hindi, Chinese, Arabic.

```html
<meta charset="UTF-8">
```

#### 3. `<meta name="viewport">` (Responsive Web Design)

* Makes your site **mobile-friendly**.
* Without this, sites may zoom out on smartphones.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

#### 4. `<meta name="description">`

* Short summary (shown in Google search results).
* Helps with **SEO & click-through rate**.

```html
<meta name="description" content="World’s best free HTML course in Urdu/Hindi by Waseem Malik. Learn from zero to hero.">
```

#### 5. Favicon

* Small icon in browser tabs, bookmarks.
* File: `favicon.ico` or PNG.

```html
<link rel="icon" type="image/png" href="favicon.png">
```

#### 6. Author & Keywords

* Tells search engines & browsers about content ownership.
* **Note:** modern SEO ignores keywords, but good for documentation.

```html
<meta name="author" content="Waseem Malik">
<meta name="keywords" content="HTML, CSS, JavaScript, Web Development, Pakistan">
```

#### 7. Open Graph Tags (Social Media Sharing)

* Control how your page looks when shared on Facebook, WhatsApp, LinkedIn.

```html
<meta property="og:title" content="Future Programming - HTML Course">
<meta property="og:description" content="Free HTML course from zero to hero in Urdu/Hindi.">
<meta property="og:image" content="thumbnail.jpg">
<meta property="og:url" content="https://futureprogramming.com/html-course">
```

#### 8. Twitter Cards (For Twitter/X)

```html
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Learn HTML Free">
<meta name="twitter:description" content="Step by step HTML in Urdu/Hindi.">
<meta name="twitter:image" content="thumbnail.jpg">
```

---

### 👨‍💻 Demo – Minimal Professional Head

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML Complete Course - Future Programming</title>
  <meta name="description" content="Learn HTML from zero to hero in Urdu/Hindi.">
  <meta name="author" content="Waseem Malik">
  <link rel="icon" href="favicon.png" type="image/png">
  <meta property="og:title" content="Future Programming - HTML Course">
  <meta property="og:description" content="Free HTML course by Waseem Malik.">
  <meta property="og:image" content="thumbnail.jpg">
  <meta property="og:url" content="https://futureprogramming.com/html-course">
</head>
<body>
  <h1>Hello World!</h1>
</body>
</html>
