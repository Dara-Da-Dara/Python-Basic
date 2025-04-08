
# 🐼 Pandas Full Class - Python Data Analysis Library

Welcome to the **Pandas Full Class**! This guide covers everything from installation to advanced data analysis using the powerful **Pandas** library in Python.

---

## 📦 Installation

```bash
pip install pandas
```

You may also need `numpy` for numerical operations:

```bash
pip install numpy
```

---

## 📘 Importing Pandas

```python
import pandas as pd
```

---

## 📊 Core Data Structures

### 1. Series

A one-dimensional labeled array.

```python
import pandas as pd

data = [10, 20, 30]
s = pd.Series(data)
print(s)
```

---

### 2. DataFrame

A two-dimensional table with rows and columns.

```python
data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35]
}
df = pd.DataFrame(data)
print(df)
```

---

## 🔍 Reading Data

### From CSV

```python
df = pd.read_csv('filename.csv')
```

### From Excel

```python
df = pd.read_excel('filename.xlsx')
```

---

## 🛠️ Basic Operations

### View Data

```python
df.head()     # First 5 rows
df.tail()     # Last 5 rows
df.info()     # Info about DataFrame
df.describe() # Summary stats
```

---

### Selection and Filtering

```python
df['Name']                 # Single column
df[['Name', 'Age']]        # Multiple columns
df[ df['Age'] > 30 ]       # Conditional filtering
```

---

### Indexing

```python
df.loc[0]                 # Label-based
df.iloc[0]                # Position-based
```

---

## ➕ Modifying Data

### Add Column

```python
df['Salary'] = [50000, 60000, 70000]
```

### Update Values

```python
df.at[0, 'Age'] = 26
```

### Delete Column

```python
df.drop('Salary', axis=1, inplace=True)
```

---

## 🔄 Handling Missing Data

```python
df.isnull()               # Check missing values
df.dropna()               # Drop missing
df.fillna(0)              # Fill with value
```

---

## 📐 Aggregations and Grouping

```python
df['Age'].mean()
df.groupby('Department')['Salary'].sum()
```

---

## 🔃 Sorting

```python
df.sort_values(by='Age')
```

---

## 🧼 Data Cleaning

```python
df.columns = df.columns.str.strip()      # Remove whitespace
df['Age'] = pd.to_numeric(df['Age'])     # Convert type
df.drop_duplicates(inplace=True)         # Drop duplicates
```

---

## 📈 Visualization (optional with matplotlib)

```bash
pip install matplotlib
```

```python
import matplotlib.pyplot as plt

df['Age'].plot(kind='hist')
plt.show()
```

---

## 📤 Exporting Data

```python
df.to_csv('output.csv', index=False)
df.to_excel('output.xlsx', index=False)
```

---

## 🧠 Tips & Tricks

- Use `df.sample(5)` to view random rows
- Use `df.memory_usage(deep=True)` to check memory
- Use `df.apply()` for row/column-wise operations

---

## 📚 References

- [Pandas Official Docs](https://pandas.pydata.org/docs/)
- [Pandas GitHub](https://github.com/pandas-dev/pandas)

---

## 🏁 Final Example

```python
import pandas as pd

data = pd.read_csv('data.csv')
data['Total'] = data['Price'] * data['Quantity']
grouped = data.groupby('Category')['Total'].sum()
print(grouped)
```

---

## 🙌 Happy Learning Pandas!
