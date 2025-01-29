# Retrieving Data from CSV and JSON Files Using Pandas  

---

## **1. Introduction to Pandas**  

**Pandas** is an open-source Python library used for:  
- **Data manipulation**
- **Data analysis**
- **Data visualization**  

It provides flexible **DataFrames**, which allow efficient data processing similar to databases.

**Exercise File:** Available at [GitHub Repository](https://github.com/team-codebug/ml-specialisation/blob/main/8_Retrieving_Data_From_CSV_And_JSON_Files.ipynb)

---

## **2. Reading CSV Files**  

**What is a CSV file?**  
- A **Comma-Separated Values (CSV) file** consists of rows of data, where each column is separated by a **comma (',')**.  
- CSV files are widely used because they store structured data in a simple, human-readable format.

### **Reading a CSV File with Pandas**  

```python
import pandas as pd

# Define file path
filepath = 'data/iris_data.csv'

# Import the data
data = pd.read_csv(filepath)

# Print the first five rows
print(data.head())
```

### **Useful Arguments for `pd.read_csv()`**
Pandas provides several useful parameters for reading CSV files in different formats:

```python
# Reading a tab-separated file (.tsv)
data = pd.read_csv(filepath, sep='\t')

# Reading a space-separated file
data = pd.read_csv(filepath, delim_whitespace=True)

# Reading a file without using the first row as column names
data = pd.read_csv(filepath, header=None)

# Specifying custom column names
data = pd.read_csv(filepath, names=['Feature1', 'Feature2', 'Feature3'])

# Handling missing values with custom indicators
data = pd.read_csv(filepath, na_values=['NA', 99])
```

---

## **3. Reading JSON Files**  

### **What is a JSON File?**
- **JavaScript Object Notation (JSON)** files store data in **key-value pairs**, similar to Python **dictionaries**.
- JSON is widely used for data exchange in web applications and APIs.

### **Reading JSON Files with Pandas**  

```python
# Read JSON file into a DataFrame
data = pd.read_json('data/sample.json')

# Write DataFrame to a JSON file
data.to_json('outputfile.json')
```

---

## **4. What is a DataFrame?**  

A **DataFrame** is the primary data structure in **Pandas** that represents tabular data in a **rows and columns format**, similar to an Excel spreadsheet or SQL table.

### **Example of a DataFrame**
| ID | Name  | Age | City       |
|----|------|----|-----------|
| 1  | Alice | 25 | New York  |
| 2  | Bob   | 30 | San Francisco |
| 3  | Charlie | 35 | Los Angeles |

- **Rows (Observations):** Each row represents a single record.
- **Columns (Features):** Each column represents an attribute of the data.

---


## **6. References**  

1. Pandas Official Documentation - [Pandas Docs](https://pandas.pydata.org/)  
2. "Python for Data Analysis" by Wes McKinney - [O'Reilly](https://www.oreilly.com/library/view/python-for-data/9781491957653/)  
3. "Automate the Boring Stuff with Python" by Al Sweigart - [Book](https://automatetheboringstuff.com/)  
4. JSON File Format - [JSON Official Site](https://www.json.org/)  

---

This document provides an overview of **reading and writing CSV & JSON files**, **data manipulation using Pandas**, and **machine learning vocabulary with a real-world example**.

