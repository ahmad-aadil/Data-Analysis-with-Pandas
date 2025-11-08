#  Introduction to Pandas

Python has become one of the most popular programming languages for **data science** — and one of the biggest reasons is its rich ecosystem of **data analysis and visualization libraries**.

Among them, **Pandas** stands out as a game-changer. It’s an open-source Python library developed by **Wes McKinney in 2008**, and today it’s considered the _standard library for data manipulation and analysis in Python._

> “Pandas offers data structures and operations for manipulating numerical tables and time series. It is free software released under the three-clause BSD license. The name is derived from the term ‘panel data’, an econometrics term for data sets that include observations over multiple time periods for the same individuals.”  
> — _Wikipedia_

In this project, we’ll explore **Pandas** and its powerful data analysis tools.

---

##  Key Features of Pandas

- Supports **reading and writing** data from multiple sources (CSV, Excel, SQL, JSON, etc.)
- Offers **data structures** like _Series_, _DataFrame_, and _Panel_ for easy data manipulation
- Handles diverse datasets — time series, tabular, heterogeneous, or matrix data
- Enables powerful operations like **subsetting, slicing, filtering, merging, joining, grouping, reshaping**, etc.
- Handles **missing data** (filling or dropping)
- Allows **data parsing and conversion**
- Includes **data filtration techniques**
- Supports **time series operations** — frequency conversion, date range generation, moving window stats, shifting, and lagging
- Integrates smoothly with **Scikit-learn, SciPy, and Statsmodels**
- Delivers **fast performance**, with optional acceleration via **Cython**

---

##  Advantages of Pandas

Pandas is at the core of Python’s data analysis stack, providing a flexible and intuitive API for working with structured data.

### 1. Data Representation

Data is represented in structures like **DataFrame** and **Series**, perfectly suited for analysis.

### 2. Easy Subsetting and Filtering

Provides clear and efficient ways to **filter, subset, and query** data.

### 3. Concise and Clear Code

Allows you to **write cleaner code**, focusing on insights instead of implementation details.

---

##  Importing Pandas

To start using Pandas, you’ll first need to import it:

```python
import pandas
```

Typically, Pandas is imported with an alias for convenience:

```python
import pandas as pd
```

It’s also common to import **NumPy**, since it supports numerical computations and underlies much of Pandas’ functionality:

```python
import numpy as np
```

**Example:**

```python
# Import pandas and numpy
import pandas as pd
import numpy as np
```

---

##  Data Structures in Pandas

Pandas provides **three main data structures** built on top of NumPy arrays — fast, flexible, and expressive.

- **Series**
- **DataFrame**
- **Panel** _(deprecated in newer versions of Pandas, but historically important)_

---

## Pandas Series

A **Series** is a **one-dimensional** labeled array capable of holding any data type (integers, strings, floats, etc.).

Think of it as a single column in an Excel sheet.

**Example:**  
A series of integers:  
`[10, 20, 30, 40, 50, 60, 70, 80, 90, 100]`

###  Key Points

- Homogeneous data
- Immutable size
- Mutable values

###  Series Constructor

```python
pandas.Series(data, index, dtype, copy)
```

**Parameters:**

- `data` → ndarray, list, dict, or scalar value
- `index` → unique, hashable labels (default: RangeIndex)
- `dtype` → optional data type
- `copy` → copy input data (default: False)

---

## Pandas DataFrame

A **DataFrame** is a **two-dimensional**, size-mutable, and heterogeneous data structure — like a spreadsheet or SQL table.

Each **column** in a DataFrame is a **Series**.

###  Key Properties

- Columns can have different data types
- Labeled axes (rows & columns)
- Mutable (columns can be added or deleted)
- Performs **arithmetic operations** on rows and columns
- Conceptually similar to a **dictionary of Series**

###  DataFrame Constructor

```python
pandas.DataFrame(data, index, columns, dtype, copy)
```

**Parameters:**

- `data` → ndarray, Series, dict, lists, or another DataFrame
- `index` → row labels (default: RangeIndex)
- `columns` → column labels
- `dtype` → optional data type
- `copy` → boolean, default False

###  Ways to Create a DataFrame

- From **lists**
- From **dictionaries**
- From **Series**
- From **NumPy arrays**
- From **another DataFrame**

---

##  Pandas Panel (3D Data)

> _Note: The Panel data structure is deprecated in modern Pandas versions. Consider using multi-index DataFrames instead._

A **Panel** was a **3D container** for data, useful for handling multiple DataFrames (like a stack of tables).

###  Axes Naming

- **items** → axis 0 (DataFrame)
- **major_axis** → axis 1 (rows)
- **minor_axis** → axis 2 (columns)

---

##  Data Import with Pandas

Pandas makes importing and exporting data ridiculously easy using its **I/O API**.

| File Type | Import Function                                      | Export Function |
| --------- | ---------------------------------------------------- | --------------- |
| CSV       | `read_csv()`                                         | `to_csv()`      |
| Excel     | `read_excel()`                                       | `to_excel()`    |
| JSON      | `read_json()`                                        | `to_json()`     |
| HTML      | `read_html()`                                        | `to_html()`     |
| SAS       | `read_sas()`                                         | —               |
| SQL       | `read_sql()`, `read_sql_query()`, `read_sql_table()` | `to_sql()`      |
| STATA     | `read_stata()`                                       | `to_stata()`    |
| Pickle    | `read_pickle()`                                      | `to_pickle()`   |
| HDF5      | `read_hdf()`                                         | `to_hdf()`      |

---

##  Conclusion

Pandas is the **backbone of data analysis in Python** — intuitive, flexible, and incredibly powerful. Whether you’re wrangling data, cleaning messy datasets, or prepping for machine learning, Pandas is the tool that gets it done.

---

### ✨ Author

**Mr. Aadil**
