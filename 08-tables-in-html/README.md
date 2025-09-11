# 📊 Chapter 08: Mastering Tables in HTML – Create a Student Result Card

Tables in HTML allow us to **organize data into rows and columns**, making information more structured and easy to understand. They are widely used for displaying data like product lists, schedules, price charts, and result cards.

In this chapter, we will learn:

* How to create tables using `<table>`, `<tr>`, `<td>`, and `<th>`
* Adding **headers, borders, captions, and styling**
* Using **rowspan** and **colspan** to merge cells
* Using **colgroup** for styling specific columns
* Building a **real-world project: A Student Result Card**

---

## 🧩 1. Basic Table Structure

A table is created with the `<table>` element.

* **Rows**: `<tr>` (table row)
* **Cells**: `<td>` (table data)
* **Headers**: `<th>` (table heading)

👉 Example:

```html
<table border="1">
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```

---

## 🏷️ 2. Table Headers

Headers are created with `<th>` instead of `<td>`.
By default, `<th>` text is **bold and centered**.

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>25</td>
    <td>Berlin</td>
  </tr>
</table>
```

---

## 🪟 3. Large Table Example (Employee List)

To understand better, let’s create a **bigger table** with multiple rows and columns:

```html
<table border="1" cellpadding="10" cellspacing="0">
  <tr>
    <th>ID</th>
    <th>Name</th>
    <th>Department</th>
    <th>Position</th>
    <th>Salary</th>
  </tr>
  <tr>
    <td>101</td>
    <td>Sarah Khan</td>
    <td>IT</td>
    <td>Developer</td>
    <td>$4000</td>
  </tr>
  <tr>
    <td>102</td>
    <td>Ali Raza</td>
    <td>HR</td>
    <td>Manager</td>
    <td>$3500</td>
  </tr>
  <tr>
    <td>103</td>
    <td>John Doe</td>
    <td>Finance</td>
    <td>Accountant</td>
    <td>$3000</td>
  </tr>
</table>
```

---

## 📌 4. Table Borders & Styling

By default, tables look plain. We can add borders and padding with **CSS**.

```html
<style>
  table, th, td {
    border: 1px solid black;
    border-collapse: collapse; /* avoid double borders */
    padding: 8px;
  }
</style>
```

---

## 🔗 5. Table Caption

We can add a title to the table using `<caption>`.

```html
<table border="1">
  <caption><b>Employee Salary Report</b></caption>
  <tr>
    <th>Name</th>
    <th>Salary</th>
  </tr>
  <tr>
    <td>Ali</td>
    <td>$3000</td>
  </tr>
</table>
```

---

## 🔄 6. Colspan & Rowspan

* **Colspan** = Merge multiple columns
* **Rowspan** = Merge multiple rows

👉 Example with **colspan**:

```html
<table border="1">
  <tr>
    <th colspan="3">Employee Info</th>
  </tr>
  <tr>
    <td>ID</td>
    <td>Name</td>
    <td>Department</td>
  </tr>
  <tr>
    <td>101</td>
    <td>Sarah</td>
    <td>IT</td>
  </tr>
</table>
```

👉 Example with **rowspan**:

```html
<table border="1">
  <tr>
    <th rowspan="2">Name</th>
    <td>Ali</td>
  </tr>
  <tr>
    <td>Ahmed</td>
  </tr>
</table>
```

---

## 🎨 7. Column Group Styling

We can apply styles to specific columns using `<colgroup>`.

```html
<table border="1">
  <colgroup>
    <col style="background-color: #f2f2f2;">
    <col style="background-color: lightblue;">
  </colgroup>
  <tr>
    <th>Name</th>
    <th>Marks</th>
  </tr>
  <tr>
    <td>Ali</td>
    <td>85</td>
  </tr>
</table>
```

---

## 📝 8. Project – Student Result Card

Now, let’s build a **real-world project** using everything we’ve learned.

```html
<style>
  table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
    padding: 8px;
    text-align: center;
  }
  caption {
    font-size: 20px;
    font-weight: bold;
    margin: 10px;
  }
</style>

<table>
  <caption>Student Result Card</caption>
  <tr>
    <th colspan="6">Student Information</th>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>Ali Raza</td>
    <td><b>Class</b></td>
    <td>10th</td>
    <td><b>Roll No</b></td>
    <td>2025</td>
  </tr>
  <tr>
    <th>Subject</th>
    <th>Marks Obtained</th>
    <th>Total Marks</th>
    <th>Grade</th>
    <th colspan="2">Remarks</th>
  </tr>
  <tr>
    <td>Math</td>
    <td>90</td>
    <td>100</td>
    <td>A+</td>
    <td colspan="2">Excellent</td>
  </tr>
  <tr>
    <td>Science</td>
    <td>85</td>
    <td>100</td>
    <td>A</td>
    <td colspan="2">Very Good</td>
  </tr>
  <tr>
    <td>English</td>
    <td>78</td>
    <td>100</td>
    <td>B+</td>
    <td colspan="2">Good</td>
  </tr>
  <tr>
    <th colspan="2">Total Marks</th>
    <th>300</th>
    <th colspan="3">253</th>
  </tr>
</table>
```

✅ This project combines:

* Headers (`<th>`)
* Colspan & Rowspan
* Captions
* Proper table styling

---

## 🎯 Key Takeaways

* Tables are perfect for organizing structured data.
* Use `<th>` for headers, `<td>` for data.
* **Colspan & Rowspan** make complex layouts possible.
* **Captions & Colgroups** enhance readability.
* With CSS, tables can be styled beautifully.
* Practical projects like a **Result Card** help you practice real-world table design.

---

👉 Now, try creating a Result Table for 3 students with at least 5 subjects each, showing percentage & overall grade.


If you’re enjoying this course:

* 📺 Watch the full HTML course playlist here: [HTML Mastery in the Age of AI (YouTube)](https://youtube.com/playlist?list=PLW52WtRpL35bDPLV_1JmeXNWGcT1qNFyf&si=J4DsLs8-F9G9GQ0N)
* ⭐ Don’t forget to **like, subscribe, and share** to support the channel.
* 💻 Practice code from our repository (coming soon in GitHub).

