# 🌍 Phase 0 — Foundations: Before Writing HTML


## 📘 Chapter 0.1 — How Computers Understand Us

### 📖 Introduction

Computers are very smart, but also very **simple-minded**.
They don’t understand **Urdu, English, Hindi, or Bengali** directly. They only understand **0 and 1** — what we call **binary language**.

To work with computers, we need a way to **convert our human language** (letters, words, emojis, numbers) into a format the computer can understand. This is the foundation of all web pages, apps, and games.

---

### 💡 Real-life Analogy

Think of a **computer like a child** who only knows how to say **yes (1)** or **no (0)**. If you say:

* “Give me water” → The child doesn’t understand.
  So, you invent a system:
* “0 = no water, 1 = water.”

Now, the child can follow you. Similarly, we convert **letters** into numbers so computers can follow our instructions.

---

### 🛠 Step-by-step Explanation

#### 1. Bits and Bytes

* A **bit** = the smallest piece of information (0 or 1).
* A **byte** = 8 bits (like 8 boxes where each box can be 0 or 1).

With bytes, we can represent letters, numbers, or even emojis.

#### 2. How Text is Stored

* Early on, English letters were stored using **ASCII** (A–Z, numbers, symbols).
* But ASCII could not store Urdu, Hindi, Chinese, or emojis.
* So, the world made **Unicode** → a system that can store almost every language.
* On the web, we use **UTF-8 encoding** → the standard that supports all characters.

Example:

* The letter **A** = number 65.
* The letter **ا** = number 0627 (in Unicode).

#### 3. Why Encoding Matters

If the computer **misunderstands encoding**, you get strange symbols like:

```
Ã© instead of é
```

This problem is called **garbled text**. To fix it, we always tell the browser:

```html
<meta charset="utf-8">
```

---

### 👨‍💻 Demo Code

```html
<!doctype html>
<html>
<head>
  <meta charset="utf-8">
  <title>Encoding Demo</title>
</head>
<body>
  <p>English: A</p>
  <p>Urdu: ا</p>
  <p>Emoji: 🙂</p>
</body>
</html>
```

👉 Save this as `index.html`, open it in a browser, and you will see that all languages and even emojis work perfectly.

---

### 🎯 Learning Outcomes

By the end of this lecture, you will:

* Understand that computers only read **0 and 1**.
* Know that **letters are stored as numbers** inside a computer.
* Learn why **UTF-8** is important for websites.
* Be able to write `<meta charset="utf-8">` in every HTML page.

