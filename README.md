# Python Data Analysis Assignment 1 – NumPy and Pandas

## 📌 Project Overview

This project demonstrates the basic concepts of **NumPy** and **Pandas** used in Python Data Analytics.

The assignment covers array operations, indexing, slicing, Pandas Series, DataFrame creation, data exploration, filtering, grouping, and data manipulation.

## 🎯 Objectives

- Create and work with NumPy arrays
- Understand array shape, data type, and size
- Perform mathematical operations using NumPy
- Perform array indexing and slicing
- Create and manipulate Pandas Series
- Understand `loc` and `iloc`
- Apply Boolean filtering
- Create and analyze Pandas DataFrames
- Perform grouping and aggregation
- Modify and delete rows and columns

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Jupyter Notebook

## 🔢 Part 1 – NumPy 1D Array

### 1.1 Creating a 1D NumPy Array

Created a 1D NumPy array named `temperature_w1` containing daily average temperature values for Week 1.

The temperature values used were:

- 22.5
- 25.3
- 20.8
- 23.4
- 26.1
- 24.8
- 21.9

### 1.2 Inspecting Array Properties

The following properties were inspected:

- Shape
- Data Type
- Number of Elements

**Result:**

- Shape: `(7,)`
- Data Type: `float64`
- Number of Elements: `7`

### 1.3 Celsius to Fahrenheit Conversion

The Celsius temperatures were converted to Fahrenheit using the formula:

**Fahrenheit = (Celsius × 9/5) + 32**

The Fahrenheit temperatures obtained were:

`72.5, 77.54, 69.44, 74.12, 78.98, 76.64, 71.42`

### 1.4 Statistical Operations

The maximum, minimum, and mean temperatures were calculated.

| Operation | Result |
|---|---:|
| Maximum Temperature | 26.1°C |
| Minimum Temperature | 20.8°C |
| Mean Temperature | 23.54°C |

## ✂️ Part 2 – NumPy Array Slicing and Indexing

### 2.1 First Three Days

The first three temperature values were extracted using array slicing.

**Result:**

`[22.5, 25.3, 20.8]`

### 2.2 Weekend Temperatures

The last two temperature values were extracted as weekend temperatures.

**Result:**

`[24.8, 21.9]`

### 2.3 Middle Three Days

The middle three temperature values were extracted.

**Result:**

`[20.8, 23.4, 26.1]`

## 📊 Part 3 – NumPy 2D Array

A 2D NumPy array named `temperatures` was created to store temperature data for two weeks.

### 3.1 Week 1 Temperature Data

`[22.5, 25.3, 20.8, 23.4, 26.1, 24.8, 21.9]`

### 3.2 Week 2 Temperature Data

`[19.2, 22.5, 21.3, 24.0, 23.5, 22.8, 20.1]`

### 3.3 Array Properties

| Property | Result |
|---|---|
| Shape | `(2, 7)` |
| Data Type | `float64` |
| Total Elements | `14` |

### 3.4 Weekly Temperature Extraction

The temperatures for Week 1 and Week 2 were extracted using array indexing.

### 3.5 Weekend Temperature Extraction

The last two days of each week were extracted.

**Week 1 Weekend:**

`[24.8, 21.9]`

**Week 2 Weekend:**

`[22.8, 20.1]`

## 🐼 Part 4 – Pandas Series

### 4.1 Creating a Pandas Series

A Pandas Series named `marks` was created using student marks and custom rank labels.

| Rank | Mark |
|---|---:|
| Rank1 | 95 |
| Rank2 | 92 |
| Rank3 | 89 |
| Rank4 | 85 |
| Rank5 | 80 |

## 🔍 Part 5 – Pandas Series Indexing and Slicing

### 5.1 Accessing the First Rank

The first-ranked student's mark was accessed using `iloc`.

**Result:**

`95`

### 5.2 Retrieving the Top Three Ranks

The top three ranks were retrieved using `loc`.

| Rank | Mark |
|---|---:|
| Rank1 | 95 |
| Rank2 | 92 |
| Rank3 | 89 |

### 5.3 Retrieving the Third Rank

The third-ranked student's mark was retrieved using `iloc`.

**Result:**

`89`

### 5.4 Filtering Marks Greater Than 90

Boolean filtering was used to find marks greater than 90.

**Result:**

- Rank1: 95
- Rank2: 92

## ✏️ Part 6 – Manipulating Pandas Series

### 6.1 Modifying Rank1 Mark

The Rank1 mark was changed from:

`95 → 100`

### 6.2 Removing Rank5

The `Rank5` entry was removed from the Series.

### 6.3 Calculating CGPA

CGPA was calculated by dividing each mark by 10.

| Rank | CGPA |
|---|---:|
| Rank1 | 10.0 |
| Rank2 | 9.2 |
| Rank3 | 8.9 |
| Rank4 | 8.5 |

## 🧾 Part 7 – Pandas DataFrame

### 7.1 Creating the DataFrame

A Pandas DataFrame named `transactions` was created to store transaction information.

The DataFrame contains the following columns:

- `TransactionID`
- `ProductCategory`
- `Region`
- `Amount`

The DataFrame contains **10 transactions**.

## 🔎 Part 8 – Data Exploration

### 8.1 DataFrame Information

The following DataFrame properties and methods were explored:

- DataFrame display
- Shape
- Column names
- Data types
- `head()`
- `tail()`

**Shape:**

`(10, 4)`

### 8.2 Selecting Product Category and Amount

The `ProductCategory` and `Amount` columns were selected from the DataFrame.

### 8.3 Selecting the Last Three Columns

The last three columns were selected using `iloc`.

The columns were:

- `ProductCategory`
- `Region`
- `Amount`

## 🔍 Part 9 – DataFrame Filtering

The DataFrame was filtered using the following conditions:

- Region = `North`
- Amount > `200`

### Matching Transactions

| TransactionID | Amount |
|---:|---:|
| 103 | 300 |
| 106 | 250 |
| 110 | 400 |

## 📊 Part 10 – Product Category Value Counts

The number of transactions in each product category was calculated using `value_counts()`.

| Product Category | Count |
|---|---:|
| Electronics | 4 |
| Clothing | 3 |
| Furniture | 3 |

## 🌍 Part 11 – Unique Regions

The unique values in the `Region` column were identified using `unique()`.

The regions were:

- North
- South
- East
- West

## 📈 Part 12 – GroupBy and Mean Calculation

The transaction data was grouped by `Region`, and the mean transaction amount was calculated.

| Region | Mean Amount |
|---|---:|
| East | 375.0 |
| North | 287.5 |
| South | 250.0 |
| West | 190.0 |

## 🛠️ Part 13 – DataFrame Manipulation

### 13.1 Modifying Transaction Amount

The Amount for TransactionID `102` was changed from:

`150 → 165`

### 13.2 Adding a Discount Column

A new column named `Discount` was created.

The discount was calculated as:

**Discount = Amount × 0.10**

### 13.3 Removing TransactionID 109

The row containing `TransactionID = 109` was removed from the DataFrame.

### 13.4 Deleting the Discount Column

The `Discount` column was deleted from the DataFrame after completing the calculation.

## 💡 Key Concepts Learned

Through this assignment, I practiced the following concepts:

- NumPy array creation
- One-dimensional arrays
- Two-dimensional arrays
- Array shape
- Array data type
- Array size
- Mathematical operations
- Celsius to Fahrenheit conversion
- Maximum value
- Minimum value
- Mean calculation
- Array indexing
- Array slicing
- Pandas Series creation
- Custom indexing
- `loc`
- `iloc`
- Boolean masking
- Series modification
- Series deletion
- CGPA calculation
- DataFrame creation
- DataFrame exploration
- Column selection
- Row filtering
- `value_counts()`
- `unique()`
- `groupby()`
- Mean aggregation
- DataFrame modification
- Adding columns
- Removing rows
- Deleting columns

## 🏁 Conclusion

This assignment provided practical experience in using **NumPy and Pandas for Python Data Analytics**.

NumPy was used to analyze weekly temperature data through array creation, mathematical operations, temperature conversion, indexing, slicing, and statistical calculations.

Pandas Series was used to analyze student marks using custom indexing, `loc`, `iloc`, Boolean filtering, modification, deletion, and CGPA calculation.

Pandas DataFrame was used to analyze transaction data through data exploration, column selection, filtering, value counts, unique values, grouping, mean calculation, row modification, column creation, row deletion, and column deletion.

Overall, this project helped me build a strong foundation in **Python Data Analytics using NumPy and Pandas**.

## 👩‍💻 Author

**Python Data Analytics Learner**


---

⭐ This project was completed as part of my Python Data Analytics learning journey.
