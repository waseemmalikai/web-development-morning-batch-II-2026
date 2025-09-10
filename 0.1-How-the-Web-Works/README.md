# 🌍 Chapter 0.2 — How the Web Works

### 📖 Introduction

The web is the system that lets you see websites on your browser. But have you ever wondered what happens when you type `www.google.com` and press Enter?

In this lesson, we’ll explain:

* How your computer talks to other computers (servers) on the internet.
* What happens behind the scenes to show you a webpage.
* Important concepts like **DNS, HTTP, HTTPS, static vs dynamic pages**.

---

### 💡 Real-life Analogy

Think of the web like sending a **letter in the mail**:

| Concept       | Analogy                                  |
| ------------- | ---------------------------------------- |
| Browser       | You (sending the letter)                 |
| URL           | Address on the envelope                  |
| DNS           | Phonebook to find the correct house (IP) |
| Server        | The house that prepares your order       |
| HTTP Request  | Letter you send                          |
| HTTP Response | Package you receive                      |

So, the web is just a **giant, super-fast postal system** for information.

---

### 🛠 Step-by-step Explanation

#### 1. DNS — How the computer finds the website

* Humans use names like `google.com`.
* Computers only understand numbers called **IP addresses** (e.g., `142.250.190.14`).
* **DNS (Domain Name System)** is like a phonebook: it converts the name to the number.

**Steps your browser follows:**

1. Check if it already knows the IP (cache).
2. Ask the operating system (OS).
3. If unknown, ask the **DNS server**.
4. Get the IP address back → now the browser can talk to the server.

---

#### 2. Client-Server Model

* **Client** = your computer or browser.
* **Server** = computer that stores website files.

**Flow:**

1. You type URL → browser is client.
2. Browser finds server IP using DNS.
3. Browser sends a **request** asking for the webpage.
4. Server sends **response** with HTML, CSS, images, etc.
5. Browser shows the page on your screen.

---

#### 3. HTTP & HTTPS

* **HTTP** = Hypertext Transfer Protocol → how browser & server talk.
* **HTTPS** = HTTP + Security (TLS encryption) → makes it safe so others can’t see your data.

**HTTP Methods (simple version):**

* `GET` → “Give me this page.”
* `POST` → “Here’s some data for you.”

**Status Codes:**

* `200` → Success
* `404` → Page not found
* `500` → Server error

---

#### 4. Static vs Dynamic Pages

* **Static pages:** HTML/CSS files served as they are.

  * Example: simple blog, personal portfolio.
* **Dynamic pages:** Server generates HTML on the fly using code.

  * Example: Facebook feed, Gmail inbox.

---

#### 5. How the browser shows the page

1. Browser gets HTML from server.
2. Creates **DOM (Document Object Model)** → tree of all elements.
3. Reads CSS → builds **CSSOM** (styles).
4. Combines DOM + CSSOM → **Render Tree** → browser calculates layout & paints pixels.
5. Executes JavaScript if any.

> Tip: Heavy JS can slow page loading, so order matters.

---

### 👨‍💻 Practical Demos

**A. Check HTTP Headers with `curl`**

```bash
curl -I https://www.google.com
```

* Look at `Content-Type` and `status` codes.

**B. Explore DevTools in Browser**

1. Open Chrome/Edge/Firefox → Press `F12`.
2. Network tab → Reload page → see requests & responses.
3. Elements tab → Inspect HTML and CSS.

**C. Simple Python HTTP Server**

```bash
# From terminal, serve current folder
python3 -m http.server 8000
# Open http://localhost:8000 in browser
```

---

### 🎯 Learning Outcomes

After this lecture you will:

* Explain how the web works in simple terms.
* Understand DNS, client-server, HTTP/HTTPS.
* Know the difference between static and dynamic websites.
* Use browser DevTools and `curl` to see requests and responses.

