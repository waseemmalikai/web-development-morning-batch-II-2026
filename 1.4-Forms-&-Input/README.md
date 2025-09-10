# 🌍 Chapter 1.4 — HTML Forms & Input Elements

### 📖 Introduction

Forms are a **core part of websites** because they allow users to **interact with your website** and **send information**.

Examples of forms:

* Contact forms
* Login / Registration forms
* Feedback forms
* Search boxes

Without forms, websites would be **static**, and users wouldn’t be able to **communicate or perform actions**.

**Key Idea:** HTML provides a **set of tags and attributes** that let us create forms, control how data is collected, and improve user experience.

---

### 💡 Real-life Analogy

Think of a form like a **paper form at a school or bank**:

* **Fields** ask for information (name, age, email).
* **Checkboxes or radio buttons** let you select options.
* **Submit button** sends the form.
* **Reset button** clears the form if you make mistakes.

The difference is that **web forms can validate data automatically** and send it instantly anywhere in the world.

---

### 🛠 Step-by-step Explanation

#### 1. The `<form>` Tag

The `<form>` tag is the **container** for all inputs.

**Basic Syntax:**

```html
<form action="submit.html" method="post">
    <!-- form elements go here -->
</form>
```

* `action` → the URL where form data will be sent.
* `method` → HTTP method for sending data:

  * `post` → sends data securely in request body.
  * `get` → sends data via URL (visible, limited).

---

#### 2. Input Fields

##### a) Text Input

```html
<label for="name">Name:</label>
<input type="text" id="name" name="name" placeholder="Enter your name" required>
```

* `type="text"` → single-line text input.
* `id` → connects label to input.
* `name` → used when sending data to the server.
* `placeholder` → shows hint inside input.
* `required` → user must fill this field.

##### b) Email Input

```html
<label for="email">Email:</label>
<input type="email" id="email" name="email" placeholder="example@mail.com" required>
```

* Browser **checks if input looks like an email** automatically.

##### c) Password Input

```html
<label for="password">Password:</label>
<input type="password" id="password" name="password" required>
```

* Hides typed characters for security.

##### d) Number Input

```html
<label for="age">Age:</label>
<input type="number" id="age" name="age" min="1" max="100" required>
```

* `min` and `max` → restrict number range.

##### e) Tel & URL Input

```html
<label for="phone">Phone:</label>
<input type="tel" id="phone" name="phone" placeholder="+92 300 1234567">

<label for="website">Website:</label>
<input type="url" id="website" name="website" placeholder="https://example.com">
```

* `tel` → for phone numbers.
* `url` → validates URL format.

---

#### 3. Checkbox & Radio Buttons

* **Checkbox** → select **multiple options**.
* **Radio** → select **only one option**.

```html
<label>Hobbies:</label>
<input type="checkbox" name="hobby" value="reading"> Reading
<input type="checkbox" name="hobby" value="sports"> Sports

<br><br>
<label>Gender:</label>
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
```

> Tip: Radio buttons with same `name` are linked, allowing only one selection.

---

#### 4. Textarea

```html
<label for="message">Message:</label>
<textarea id="message" name="message" rows="5" cols="50" placeholder="Write your message"></textarea>
```

* `rows` → height in lines.
* `cols` → width in characters.
* Used for **long text input**, like feedback or comments.

---

#### 5. Select Dropdown

```html
<label for="country">Country:</label>
<select id="country" name="country">
    <option value="pakistan">Pakistan</option>
    <option value="india">India</option>
    <option value="bangladesh">Bangladesh</option>
</select>
```

* `<select>` → dropdown menu.
* `<option>` → each selectable item.

---

#### 6. Form Buttons

```html
<input type="submit" value="Submit">
<input type="reset" value="Reset">
```

* `submit` → sends form data to server.
* `reset` → clears all inputs.

---

#### 7. Additional Input Attributes

| Attribute   | Use                                     |
| ----------- | --------------------------------------- |
| `autofocus` | Focus cursor automatically on page load |
| `disabled`  | Field cannot be edited                  |
| `readonly`  | Field can be seen but not edited        |
| `maxlength` | Limits number of characters             |
| `pattern`   | Regex pattern to validate input         |

**Example:**

```html
<input type="text" name="username" maxlength="15" pattern="[A-Za-z0-9]+" required placeholder="Enter username">
```

---

#### 8. Grouping Inputs with `<fieldset>` & `<legend>`

```html
<fieldset>
    <legend>Personal Info</legend>
    <label for="fname">First Name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    
    <label for="lname">Last Name:</label>
    <input type="text" id="lname" name="lname">
</fieldset>
```

* `<fieldset>` → groups related fields.
* `<legend>` → title for the group.
* Improves **form structure and readability**.

---

### 👨‍💻 Practical Demo

```html
<h2>Contact Form</h2>
<form action="submit.html" method="post">
    <fieldset>
        <legend>Personal Information</legend>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" placeholder="Your Name" required><br><br>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" placeholder="example@mail.com" required><br><br>
        
        <label for="age">Age:</label>
        <input type="number" id="age" name="age" min="1" max="100"><br><br>
        
        <label>Gender:</label>
        <input type="radio" name="gender" value="male"> Male
        <input type="radio" name="gender" value="female"> Female<br><br>
        
        <label>Hobbies:</label>
        <input type="checkbox" name="hobby" value="reading"> Reading
        <input type="checkbox" name="hobby" value="sports"> Sports<br><br>
        
        <label for="country">Country:</label>
        <select id="country" name="country">
            <option value="pakistan">Pakistan</option>
            <option value="india">India</option>
            <option value="bangladesh">Bangladesh</option>
        </select><br><br>
        
        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="5" cols="50" placeholder="Your message"></textarea><br><br>
    </fieldset>
    
    <input type="submit" value="Submit">
    <input type="reset" value="Reset">
</form>
```

* Open in **Live Server**, fill the form, and see **how every input works**.

---

### 🎯 Learning Outcomes

After this lecture, students will be able to:

* Create **complete forms** with text, email, password, number, radio, checkbox, and dropdown inputs.
* Use **labels, placeholders, and textareas** effectively.
* Group inputs using `<fieldset>` and `<legend>`.
* Apply **form validation** using `required`, `min`, `max`, and `pattern`.
* Understand **submit and reset buttons**, and **best practices** for form usability.