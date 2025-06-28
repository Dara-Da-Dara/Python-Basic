
# 🧠 Gradio Data Explorer – Input Guide

This guide explains what inputs to provide in the Gradio interface built with dummy Pandas data.

---

## 🎯 Input Fields in the Gradio App

### 1. **Task (Dropdown)**
Choose one of the following tasks:

| Task Name        | Description |
|------------------|-------------|
| **Show Head**     | View the first 5 rows of the dataset |
| **Show Shape**    | See number of rows and columns |
| **Show Columns**  | See list of all column names |
| **Describe**      | Get statistical summary (mean, std, count, etc.) |
| **Check Nulls**   | See count of missing values per column |
| **Filter Rows**   | Filter rows where a column contains a keyword |

---

### 2. **Column (Textbox)**
*(Only required for "Filter Rows")*

Enter the exact column name from the dataset:
- `Name`
- `Age`
- `Department`
- `Salary`
- `JoinDate`

---

### 3. **Filter Value (Textbox)**
*(Only required for "Filter Rows")*

Enter the value to filter on. Case-insensitive, partial match works.

---

## 🔍 Example Inputs

| Task         | Column      | Filter Value |
|--------------|-------------|---------------|
| Show Head    | *(leave blank)* | *(leave blank)* |
| Show Shape   | *(leave blank)* | *(leave blank)* |
| Show Columns | *(leave blank)* | *(leave blank)* |
| Describe     | *(leave blank)* | *(leave blank)* |
| Check Nulls  | *(leave blank)* | *(leave blank)* |
| Filter Rows  | Department   | HR |
| Filter Rows  | Name         | a |

---

## ✅ Example: Filtering

If you input:

- Task: `Filter Rows`  
- Column: `Department`  
- Filter Value: `HR`  

👉 The app will display all employees in the HR department.

---

## 💡 Tip

To avoid typos when entering column names, consider modifying the Gradio UI to use a **dropdown for columns**.

---
