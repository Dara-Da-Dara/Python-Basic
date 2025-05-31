
# 🐼 Pandas Exercise and Solution

This exercise demonstrates basic Pandas operations on a simple sales dataset.

---

## 📊 Sample Data

```python
import pandas as pd

data = {
    'Date': ['2025-01-01', '2025-01-02', '2025-01-03', '2025-01-04', '2025-01-05'],
    'Product': ['A', 'B', 'A', 'C', 'B'],
    'Units Sold': [10, 15, 8, 12, 7],
    'Unit Price': [20, 30, 20, 25, 30]
}

df = pd.DataFrame(data)
```

---

## ✅ Tasks

1. Convert the `Date` column to `datetime`.
2. Add a new column `Total Sales` (`Units Sold × Unit Price`).
3. Filter the rows where `Product` is `'B'`.
4. Group the data by `Product` and calculate total `Units Sold` and `Total Sales`.
5. Sort the data by `Total Sales` in descending order.
6. Find the product with the highest total sales.

---

## 🧠 Solution

```python
import pandas as pd

# Step 1: Create the DataFrame
data = {
    'Date': ['2025-01-01', '2025-01-02', '2025-01-03', '2025-01-04', '2025-01-05'],
    'Product': ['A', 'B', 'A', 'C', 'B'],
    'Units Sold': [10, 15, 8, 12, 7],
    'Unit Price': [20, 30, 20, 25, 30]
}

df = pd.DataFrame(data)

# Step 2: Convert 'Date' column to datetime
df['Date'] = pd.to_datetime(df['Date'])

# Step 3: Add 'Total Sales' column
df['Total Sales'] = df['Units Sold'] * df['Unit Price']

# Step 4: Filter rows where Product == 'B'
product_b_df = df[df['Product'] == 'B']

# Step 5: Group by Product and calculate totals
grouped_df = df.groupby('Product').agg({
    'Units Sold': 'sum',
    'Total Sales': 'sum'
}).reset_index()

# Step 6: Sort by 'Total Sales' in descending order
sorted_df = grouped_df.sort_values(by='Total Sales', ascending=False)

# Step 7: Find the product with the highest total sales
top_product = sorted_df.iloc[0]

# Displaying outputs
print("Original DataFrame:\n", df, "\n")
print("Filtered DataFrame (Product B):\n", product_b_df, "\n")
print("Grouped and Aggregated DataFrame:\n", grouped_df, "\n")
print("Sorted by Total Sales:\n", sorted_df, "\n")
print("Product with Highest Total Sales:\n", top_product, "\n")
```

---

Would you like to add a visualization (bar chart) for product-wise total sales?

