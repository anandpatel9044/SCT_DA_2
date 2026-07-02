# 🧹 Data Cleaning and Preparation using Python (Pandas)

This project demonstrates the process of cleaning and preparing the **Global Superstore** dataset using **Python** and the **Pandas** library. The objective is to improve data quality by checking for missing values, removing duplicate records, converting data types, and exporting the cleaned dataset for further analysis.

---

## 📌 Project Overview

Data cleaning is an essential step in the data analysis process. In this project, the Global Superstore dataset is loaded into a Jupyter Notebook, cleaned using Pandas, and exported as a new CSV file.

---

## 🎯 Objectives

- Load the Global Superstore dataset.
- Inspect dataset structure and data types.
- Identify missing values.
- Remove duplicate records.
- Convert date columns to datetime format.
- Export the cleaned dataset as a new CSV file.

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- Jupyter Notebook

---

## 📂 Dataset

**Dataset:** Global Superstore.csv

### Dataset Features

- Category
- City
- Country
- Customer ID
- Customer Name
- Discount
- Market
- Order Date
- Order ID
- Order Priority
- Product ID
- Product Name
- Profit
- Quantity
- Region
- Sales
- Segment
- Ship Date
- Ship Mode
- Shipping Cost
- State
- Sub-Category
- Year

---

## 🧹 Data Cleaning Steps

### 1️⃣ Import Pandas

```python
import pandas as pd
```

### 2️⃣ Load Dataset

```python
df = pd.read_csv("Global Superstore.csv")
```

### 3️⃣ Display First Five Rows

```python
df.head()
```

### 4️⃣ Check Dataset Information

```python
df.info()
```

### 5️⃣ Check Missing Values

```python
df.isnull().sum()
```

**Result:**

- No missing values found.

### 6️⃣ Remove Missing Values

```python
df = df.dropna()
```

### 7️⃣ Check Duplicate Records

```python
df.duplicated().sum()
```

**Result:**

- No duplicate rows found.

### 8️⃣ Remove Duplicate Records

```python
df = df.drop_duplicates()
```

### 9️⃣ Check Data Types

```python
df.dtypes
```

### 🔟 Convert Date Columns

```python
df["Order Date"] = pd.to_datetime(df["Order Date"])
df["Ship Date"] = pd.to_datetime(df["Ship Date"])
```

### 1️⃣1️⃣ Export Cleaned Dataset

```python
df.to_csv("Cleaned_Global_Superstore.csv", index=False)
```

---

## ✅ Results

- Dataset loaded successfully.
- No missing values found.
- No duplicate records found.
- Converted **Order Date** and **Ship Date** into datetime format.
- Cleaned dataset exported successfully.

---

## 📁 Project Structure

```
SCT_DA_2/
│── Global Superstore.csv
│── Cleaned_Global_Superstore.csv
│── Data_Cleaning.ipynb
└── README.md
```

---

## 📊 Output

The cleaned dataset is saved as:

```
Cleaned_Global_Superstore.csv
```

This dataset is ready for:

- Data Analysis
- Dashboard Creation
- Machine Learning
- Business Intelligence

---

## 📚 Skills Demonstrated

- Python Programming
- Pandas
- Data Cleaning
- Data Preprocessing
- Data Validation
- Data Type Conversion
- CSV File Handling
- Jupyter Notebook

---

## 🚀 How to Run

1. Clone this repository.

```bash
git clone https://github.com/anandpatel9044/SCT_DA_2.git
```

2. Install Pandas.

```bash
pip install pandas
```

3. Open Jupyter Notebook.

```bash
jupyter notebook
```

4. Run all cells in **Data_Cleaning.ipynb**.

---

## 👨‍💻 Author

**Anand Patel**

- GitHub: https://github.com/anandpatel9044
- LinkedIn: www.linkedin.com/in/anand-patel17

---

## ⭐ If you found this project helpful, don't forget to star the repository!
