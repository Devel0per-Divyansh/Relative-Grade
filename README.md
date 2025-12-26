# 📊 Relative Grade Calculator

A clean, modern **web-based Relative Grade Calculator** that assigns grades based on **class performance percentiles** instead of fixed cutoffs.  
Designed especially for universities and institutions following **relative grading systems**.

---

## 🚀 Features

- 📂 **Excel / CSV Upload**
  - Supports `.xlsx`, `.xls`, and `.csv` files
  - Automatically detects columns

- 🎯 **Percentile-Based Grading**
  - S grade assigned to top *N%* students
  - Remaining students divided into **A → E** grades
  - Below threshold → **U (Fail)**

- 📈 **Dynamic Grade Thresholds**
  - Automatically calculates grade cutoffs
  - Prevents invalid configurations (e.g., S < fail threshold)

- 📊 **Visual Analytics**
  - Grade distribution summary
  - Interactive **SVG line chart** for grade counts

- 🌗 **Dark / Light Mode**
  - Persistent theme using localStorage

- 📥 **Export Results**
  - Download final graded results as an Excel file

- 💡 **No Backend Required**
  - Runs entirely in the browser
  - No frameworks, no server, no dependencies (except XLSX)

---

## 🧠 Grading Algorithm (Simplified)

1. Sort all valid marks (0–100) in descending order  
2. Assign **S grade** to top *X%* students  
3. Define **Fail Threshold** (default: 40)  
4. Divide remaining range `(S_min − Fail)` into **5 equal bands**
   - A → B → C → D → E  
5. Marks below threshold → **U grade**

---

## 🛠 Tech Stack

- **HTML5**
- **CSS3**
  - CSS Variables
  - Grid & Flexbox
- **Vanilla JavaScript**
- **SheetJS (XLSX.js)** for Excel parsing
- **SVG** for charts

---

## 📂 File Structure

```text
relative-grade-calculator/
│
├── index.html      # Complete application
├── README.md       # Documentation
