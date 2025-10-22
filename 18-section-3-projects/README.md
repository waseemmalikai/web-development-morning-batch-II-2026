# 🎓 **Chapter 18: Section 3 Projects — Layouts Like a Pro**

**Real-World Responsive Layout Projects with Flexbox + Grid**

---

## 🧠 **What You’ll Learn**

By the end of this chapter, you’ll be able to:

* Design and build **modern responsive layouts** using Flexbox, Grid, and Media Queries.
* Recreate professional UI sections used by real websites.
* Combine your layout knowledge into full-page responsive designs.
* Understand how designers and developers structure modern pages.

---

## 💡 **Chapter Theme: “From Designer to Developer — Bringing Layouts to Life”**

Imagine you’ve just been hired by a new tech startup.
They need a **SaaS landing page**, a **portfolio**, a **blog**, an **eCommerce layout**, and a **dashboard** — all responsive and modern.

Your task? Build each one from scratch — no frameworks, just CSS superpowers 💪

Let’s begin your layout mission. 🚀

---

# 🧩 **Project 1: SaaS Startup Pricing Section (Flexbox + Media Queries)**

### 🎯 Goal:

Build a clean, responsive **pricing section** like you see on SaaS landing pages (e.g., Notion, Canva, or Figma).

---

### 🧱 **HTML Structure**

```html
<section class="pricing">
  <h2>Choose Your Plan</h2>
  <div class="pricing-cards">
    <div class="card">
      <h3>Basic</h3>
      <p>$9/month</p>
      <ul>
        <li>✔ 10 Projects</li>
        <li>✔ 5 GB Storage</li>
        <li>✔ Email Support</li>
      </ul>
      <button>Get Started</button>
    </div>

    <div class="card highlight">
      <h3>Pro</h3>
      <p>$29/month</p>
      <ul>
        <li>✔ 50 Projects</li>
        <li>✔ 50 GB Storage</li>
        <li>✔ Priority Support</li>
      </ul>
      <button>Go Pro</button>
    </div>

    <div class="card">
      <h3>Enterprise</h3>
      <p>$99/month</p>
      <ul>
        <li>✔ Unlimited Projects</li>
        <li>✔ 1 TB Storage</li>
        <li>✔ Dedicated Support</li>
      </ul>
      <button>Contact Sales</button>
    </div>
  </div>
</section>
```

---

### 🎨 **CSS**

```css
.pricing {
  text-align: center;
  padding: 60px 20px;
  background: #f9f9f9;
}

.pricing-cards {
  display: flex;
  justify-content: center;
  gap: 30px;
  flex-wrap: wrap;
}

.card {
  background: white;
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  width: 300px;
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-10px);
}

.card.highlight {
  background: linear-gradient(135deg, #4facfe, #00f2fe);
  color: white;
}

button {
  margin-top: 20px;
  padding: 12px 20px;
  border: none;
  border-radius: 8px;
  background: #333;
  color: white;
  cursor: pointer;
}

/* Responsive */
@media (max-width: 768px) {
  .pricing-cards {
    flex-direction: column;
    align-items: center;
  }
}
```

✅ Mobile-ready, visually balanced, and perfect for landing pages.

---

# 🧩 **Project 2: Portfolio Grid Gallery (CSS Grid + Responsive Images)**

### 🎯 Goal:

Showcase creative projects in a **masonry-style grid layout** that adapts beautifully on all screens.

---

### 🧱 **HTML**

```html
<section class="portfolio">
  <h2>My Work</h2>
  <div class="grid-gallery">
    <img src="img1.jpg" alt="">
    <img src="img2.jpg" alt="">
    <img src="img3.jpg" alt="">
    <img src="img4.jpg" alt="">
    <img src="img5.jpg" alt="">
    <img src="img6.jpg" alt="">
  </div>
</section>
```

---

### 🎨 **CSS**

```css
.portfolio {
  text-align: center;
  padding: 60px 20px;
}

.grid-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 15px;
}

.grid-gallery img {
  width: 100%;
  border-radius: 10px;
  transition: transform 0.3s;
}

.grid-gallery img:hover {
  transform: scale(1.05);
}
```

✅ Uses `auto-fit` and `minmax()` for responsive image grids — no media queries needed!

---

# 🧩 **Project 3: Blog Layout (Grid + Flexbox)**

### 🎯 Goal:

Design a responsive blog layout with a **main content area** and **sidebar**.

---

### 🧱 **HTML**

```html
<section class="blog">
  <div class="main">
    <article>
      <h2>Latest Trends in CSS</h2>
      <p>CSS is evolving faster than ever...</p>
    </article>
    <article>
      <h2>10 Flexbox Tricks You Must Know</h2>
      <p>Flexbox simplifies alignment...</p>
    </article>
  </div>

  <aside class="sidebar">
    <h3>Categories</h3>
    <ul>
      <li>CSS</li><li>HTML</li><li>Design</li>
    </ul>
  </aside>
</section>
```

---

### 🎨 **CSS**

```css
.blog {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 30px;
  padding: 40px;
}

.sidebar {
  background: #f0f0f0;
  padding: 20px;
  border-radius: 10px;
}

@media (max-width: 768px) {
  .blog {
    grid-template-columns: 1fr;
  }
}
```

✅ Adapts from two columns to one column on mobile.

---

# 🧩 **Project 4: E-commerce Website Layout**

### 🎯 Goal:

Create a responsive **product grid layout** with image, name, and price — just like online stores.

---

### 🧱 **HTML**

```html
<section class="products">
  <h2>Shop Our Collection</h2>
  <div class="product-grid">
    <div class="product">
      <img src="shirt.jpg" alt="">
      <h3>Blue Shirt</h3>
      <p>$25</p>
    </div>
    <div class="product">
      <img src="watch.jpg" alt="">
      <h3>Smart Watch</h3>
      <p>$79</p>
    </div>
    <div class="product">
      <img src="headphones.jpg" alt="">
      <h3>Wireless Headphones</h3>
      <p>$59</p>
    </div>
  </div>
</section>
```

---

### 🎨 **CSS**

```css
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  padding: 20px;
}

.product {
  background: #fff;
  text-align: center;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.product img {
  width: 100%;
  border-radius: 10px;
}
```

✅ Fully responsive and reusable for real eCommerce projects.

---

# 🧩 **Project 5: Dashboard Layout (Grid + Sidebar + Topbar)**

### 🎯 Goal:

Build a **dashboard-style layout** — perfect for admin panels or analytics pages.

---

### 🧱 **HTML**

```html
<div class="dashboard">
  <aside class="sidebar">
    <h2>Dashboard</h2>
    <ul>
      <li>Overview</li>
      <li>Reports</li>
      <li>Settings</li>
    </ul>
  </aside>

  <main class="main">
    <header class="topbar">Welcome, User 👋</header>
    <section class="cards">
      <div class="card">Sales</div>
      <div class="card">Users</div>
      <div class="card">Revenue</div>
    </section>
  </main>
</div>
```

---

### 🎨 **CSS**

```css
.dashboard {
  display: grid;
  grid-template-columns: 250px 1fr;
  height: 100vh;
}

.sidebar {
  background: #333;
  color: white;
  padding: 20px;
}

.main {
  background: #f9f9f9;
  display: flex;
  flex-direction: column;
}

.topbar {
  background: white;
  padding: 15px 25px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  padding: 20px;
}

.card {
  background: white;
  padding: 30px;
  border-radius: 10px;
  text-align: center;
  box-shadow: 0 5px 10px rgba(0,0,0,0.1);
}

/* Responsive */
@media (max-width: 768px) {
  .dashboard {
    grid-template-columns: 1fr;
  }
  .sidebar {
    display: none;
  }
}
```

✅ Scales from desktop dashboard to clean mobile view.

---

# 🌍 **Final Summary**

You’ve now completed **five real-world responsive layout projects**:

1. 💰 SaaS Pricing Section (Flexbox)
2. 🎨 Portfolio Grid Gallery (Grid)
3. 📰 Blog Layout (Grid + Flexbox)
4. 🛒 E-commerce Product Grid
5. 📊 Dashboard Layout (Grid + Sidebar + Topbar)

---

## 🚀 **Bonus Ideas**

* Combine all projects into a single **Portfolio Website**.
* Add **Dark Mode** support using CSS variables.
* Animate layout transitions using `@keyframes` or `transition`.
