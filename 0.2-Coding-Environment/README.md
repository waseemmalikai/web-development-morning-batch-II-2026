# 🌍 Chapter 0.3 — Setting Up Your HTML Coding Environment

### 📖 Introduction

Before writing HTML, we need a **place to write and run our code**.
You **can** use Notepad (Windows) or TextEdit (Mac) to write HTML, but **professionals use IDEs** (Integrated Development Environments) or **code editors**.

A good coding environment helps you:

* Write code **faster** and **cleaner**.
* See your changes in **real-time**.
* Avoid errors with **auto-completion and suggestions**.

For HTML, the **most popular editor** is **VS Code (Visual Studio Code)**.

---

### 💡 Real-life Analogy

Think of writing HTML like **building a house**:

* Notepad = bare tools (hammer, nails) → you can build, but it’s slow.
* VS Code = fully equipped workshop with power tools, measuring tape, and safety gear → faster, easier, and fewer mistakes.

---

### 🛠 Step-by-step Explanation

#### 1. Install VS Code

1. Go to [VS Code official website](https://code.visualstudio.com/).
2. Download the version for your operating system (Windows, Mac, Linux).
3. Run the installer → use default settings.

#### 2. Install Useful Extensions

Extensions make coding **faster and smarter**.

**Recommended Extensions for HTML:**

* **Live Server** → see changes in the browser instantly.
* **Prettier** → automatically formats your code.
* **HTML CSS Support** → better auto-complete for CSS classes.
* **Icons / Themes** → for better visuals.

**How to Install Extensions:**

1. Open VS Code → Click on the **Extensions icon** (left sidebar).
2. Search for extension name → Click **Install**.

---

#### 3. Set Up Your First Project Folder

1. Create a folder on your computer → name it `HTML_Course`.
2. Inside the folder, create a file → `index.html`.
3. Open the folder in VS Code → `File → Open Folder`.

---

#### 4. Boilerplate HTML Code

Instead of writing everything manually, we can use **Emmet** (built into VS Code).

Type `!` and press **Tab**, VS Code will create:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

> This is called the **HTML boilerplate** — a starting template for every page.

---

#### 5. Start Live Server

1. Right-click on `index.html` → Click **Open with Live Server**.
2. A browser will open → shows your webpage.
3. Any changes in VS Code → automatically refresh in the browser.

---

#### 6. Useful VS Code Shortcuts

* **Copy line down** → `Shift + Alt + DownArrow`
* **Comment/Uncomment line** → `Ctrl + /`
* **Format code** → `Shift + Alt + F`

These shortcuts will **save a lot of time** as you write more HTML.

---

#### 7. Optional: Set Up Folder Structure

As projects grow, keep files organized:

```
HTML_Course/
├─ index.html
├─ css/
│   └─ style.css
├─ js/
│   └─ script.js
└─ images/
```

> This makes it easier to manage files for **bigger websites**.

---

### 👨‍💻 Practical Demo

1. Open VS Code → create `index.html`.
2. Type `!` → press Tab → boilerplate appears.
3. Save → Open with Live Server.
4. Type `<h1>Hello World!</h1>` in `<body>` → see it in browser instantly.

```html
<body>
    <h1>Hello World!</h1>
    <p>Welcome to your first web page!</p>
</body>
```

---

### 🎯 Learning Outcomes

By the end of this lecture, you will:

* Understand why **VS Code** is better than Notepad for HTML.
* Install VS Code and **essential extensions**.
* Create your first HTML project folder and file.
* Use **boilerplate code** to start quickly.
* Run your webpage using **Live Server**.
* Use basic shortcuts to write code faster.

