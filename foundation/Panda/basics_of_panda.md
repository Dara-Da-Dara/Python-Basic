
Importing Pandas
python
Copy
Edit
import pandas as pd
🔹 Pandas Series
A Series is a one-dimensional array with axis labels.

python
Copy
Edit
import pandas as pd

# Creating a Series
marks = [85, 90, 78, 92]
series = pd.Series(marks, index=['Arun', 'Divya', 'Lakshmi', 'Rajesh'])

print(series)
Output:

go
Copy
Edit
Arun       85
Divya      90
Lakshmi    78
Rajesh     92
dtype: int64
🔸 Pandas DataFrame
A DataFrame is a two-dimensional tabular data structure with labeled axes.

python
Copy
Edit
# Creating a DataFrame with Indian data
data = {
    'Name': ['Arun', 'Lakshmi', 'Ravi', 'Divya'],
    'Age': [24, 27, 22, 29],
    'City': ['Chennai', 'Hyderabad', 'Bangalore', 'Kochi']
}

df = pd.DataFrame(data)
print(df)
Output:

markdown
Copy
Edit
     Name  Age       City
0    Arun   24    Chennai
1  Lakshmi   27  Hyderabad
2    Ravi   22  Bangalore
3   Divya   29      Kochi
📂 Reading Data from Files
python
Copy
Edit
# Reading a CSV file
df = pd.read_csv('students_data.csv')

# Reading an Excel file
df = pd.read_excel('students_data.xlsx')
🛠️ Basic Operations
python
Copy
Edit
# First few rows
df.head()

# Last few rows
df.tail()

# Summary statistics
df.describe()

# Column data types
df.dtypes

# Access a specific column
df['City']

# Filter rows where Age > 25
df[df['Age'] > 25]
🔄 Data Cleaning
python
Copy
Edit
# Check for missing values
df.isnull().sum()

# Fill missing values with default
df.fillna('Unknown', inplace=True)

# Drop rows with any missing values
df.dropna(inplace=True)

# Rename columns
df.rename(columns={'Name': 'Student Name'}, inplace=True)

# Change data type
df['Age'] = df['Age'].astype(int)
📊 Aggregation
python
Copy
Edit
# Count of students per city
df['City'].value_counts()

# Average age by city
df.groupby('City')['Age'].mean()
📈 Visualization
python
Copy
Edit
import matplotlib.pyplot as plt

# Bar plot of age
df['Age'].plot(kind='bar', title='Student Ages')
plt.xlabel('Index')
plt.ylabel('Age')
plt.show()
📝 Summary Table
Feature	Description
Series	1D labeled array
DataFrame	2D table of rows and columns
I/O	Read/write CSV, Excel, JSON etc.
Cleaning	Fill/drop nulls, rename, type change
Filtering	Subset based on conditions
Grouping	Aggregate by column(s)
Plotting	Quick plots with .plot()
🚀 Practice Task
🧠 Challenge:

Load a dataset of students from South India.

Filter out students from Bangalore.

Plot a pie chart showing count of students per city.

python
Copy
Edit
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv('south_indian_students.csv')

# Filter Bangalore students
bangalore_students = df[df['City'] == 'Bangalore']

# City-wise count
df['City'].value_counts().plot(kind='pie', autopct='%1.1f%%')
plt.title('Student Distribution by City')
plt.ylabel('')
plt.show()
📚 References
🔗 Pandas Documentation

🔗 Cheat Sheet (PDF)

Happy Learning with Pandas! 🇮🇳🐼📘

yaml
Copy
Edit

---

If you'd like me to export this to a downloadable `.md` file or include realistic sample CSV/Excel data of Indian students, just let me know!
You said:
give full markdown code , combined 
ChatGPT said:
Absolutely! Below is the complete combined Markdown code you can copy into a .md file (e.g., pandas_class_indian.md). It’s tailored with South Indian names, Indian city data, and appropriate examples — all in one well-structured document:

markdown
Copy
Edit
# 📊 Introduction to Pandas in Python (with Indian Data)

## 🐼 What is Pandas?

**Pandas** is a powerful open-source data analysis and manipulation tool built on top of Python. It provides fast, flexible, and expressive data structures for working with structured (tabular, multidimensional) and time series data.

---

## 📦 Installation

Install Pandas using pip:

```bash
pip install pandas
✍️ Importing Pandas
python
Copy
Edit
import pandas as pd
🔹 Pandas Series
A Series is a one-dimensional array with axis labels.

python
Copy
Edit
import pandas as pd

# Creating a Series
marks = [85, 90, 78, 92]
series = pd.Series(marks, index=['Arun', 'Divya', 'Lakshmi', 'Rajesh'])

print(series)
Output:

go
Copy
Edit
Arun       85
Divya      90
Lakshmi    78
Rajesh     92
dtype: int64
🔸 Pandas DataFrame
A DataFrame is a two-dimensional tabular data structure with labeled axes.

python
Copy
Edit
# Creating a DataFrame with Indian data
data = {
    'Name': ['Arun', 'Lakshmi', 'Ravi', 'Divya'],
    'Age': [24, 27, 22, 29],
    'City': ['Chennai', 'Hyderabad', 'Bangalore', 'Kochi']
}

df = pd.DataFrame(data)
print(df)
Output:

markdown
Copy
Edit
     Name  Age       City
0    Arun   24    Chennai
1  Lakshmi   27  Hyderabad
2    Ravi   22  Bangalore
3   Divya   29      Kochi
📂 Reading Data from Files
python
Copy
Edit
# Reading a CSV file
df = pd.read_csv('students_data.csv')

# Reading an Excel file
df = pd.read_excel('students_data.xlsx')
🛠️ Basic Operations
python
Copy
Edit
# First few rows
df.head()

# Last few rows
df.tail()

# Summary statistics
df.describe()

# Column data types
df.dtypes

# Access a specific column
df['City']

# Filter rows where Age > 25
df[df['Age'] > 25]
🔄 Data Cleaning
python
Copy
Edit
# Check for missing values
df.isnull().sum()

# Fill missing values with default
df.fillna('Unknown', inplace=True)

# Drop rows with any missing values
df.dropna(inplace=True)

# Rename columns
df.rename(columns={'Name': 'Student Name'}, inplace=True)

# Change data type
df['Age'] = df['Age'].astype(int)
📊 Aggregation
python
Copy
Edit
# Count of students per city
df['City'].value_counts()

# Average age by city
df.groupby('City')['Age'].mean()
📈 Visualization
python
Copy
Edit
import matplotlib.pyplot as plt

# Bar plot of age
df['Age'].plot(kind='bar', title='Student Ages')
plt.xlabel('Index')
plt.ylabel('Age')
plt.show()
📝 Summary Table
Feature	Description
Series	1D labeled array
DataFrame	2D table of rows and columns
I/O	Read/write CSV, Excel, JSON etc.
Cleaning	Fill/drop nulls, rename, type change
Filtering	Subset based on conditions
Grouping	Aggregate by column(s)
Plotting	Quick plots with .plot()
🚀 Practice Task
🧠 Challenge:

Load a dataset of students from South India.

Filter out students from Bangalore.

Plot a pie chart showing count of students per city.

python
Copy
Edit
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv('south_indian_students.csv')

# Filter Bangalore students
bangalore_students = df[df['City'] == 'Bangalore']

# City-wise count
df['City'].value_counts().plot(kind='pie', autopct='%1.1f%%')
plt.title('Student
