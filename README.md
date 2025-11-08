**Introduction to Pandas**
Today, Python is considered as the most popular programming language for doing data science work. The reason behind this popularity is that Python provides great packages for doing data analysis and visualization work.

Pandas is one of those packages that makes analysing data much easier. Pandas is an open source library for data analysis in Python. It was developed by Wes McKinney in 2008. Over the years, it has become the standard library for data analysis using Python.

According to the Wikipedia page on Pandas,

"Pandas offers data structures and operations for manipulating numerical tables and time series. It is free software released under the three-clause BSD license. The name is derived from the term 'panel data', an econometrics term for data sets that include observations over multiple time periods for the same individuals."

In this project, I explore Pandas and various data analysis tools provided by Pandas.

**Key features of Pandas**
Some key features of Pandas are as follows:-

It provides tools for reading and writing data from a wide variety of sources such as CSV files, excel files, databases such as SQL, JSON files.

It provides different data structures like series, dataframe and panel for data manipulation and indexing.

It can handle wide variety of data sets in different formats – time series, heterogeneous data, tabular and matrix data.

It can perform variety of operations on datasets. It includes subsetting, slicing, filtering, merging, joining, groupby,
reordering and reshaping operations.

It can deal with missing data by either deleting them or filling them with zeros or a suitable test statistic.

It can be used for parsing and conversion of data.

It provides data filtration techniques.

It provides time series functionality – date range generation, frequency conversion, moving window statistics, data shifting and lagging.

It integrates well with other Python libraries such as Scikit-learn, statsmodels and SciPy.

It delivers fast performance. Also, it can be speeded up even more by making use of Cython (C extensions to Python).
**Advantages of Pandas**
Pandas is a core component of the Python data analysis toolkit. Pandas provides data structure and operations facilities, which is particularly useful for data analysis. There are various advantages of using Pandas for data analysis.

These advantages are as follows:-

Data representation
It represents data in a form that is very much suited for data analysis through its Dataframe and Series data structures. 2. Data subsetting and filtering

It provides for easy subsetting and filtering of data. It provides procedures that are suited for data analysis. 3. Concise and clear code

It provides functionality to write clear and concise code. It allows us to focus on the task at hand, rather than have to write tedious code.

**Importing Pandas**
In order to use Pandas in our work, we need to import the Pandas library first. We can import the Pandas library with the following command:-

import pandas

Usually, we import the Pandas library by appending the alias as pd. It makes things easier because now instead of writing pandas.command we need to write pd.command. So, we will import pandas with the following command:-

import pandas as pd

Also, I will import Numpy as well, because it is very useful library for scientific computing with Python. I will import Numpy with the following command:-

import numpy as np

# import pandas and numpy

import pandas as pd

import numpy as np
**Data structures in Pandas**
Pandas provide easy to use data structures.

There are three main data structures in Pandas. They are:-

Series

Dataframe

Panel

These data structures are built on top of Numpy array, which means they are fast. I have described these data structures in the following sections.

**Pandas Series**
A Pandas Series is a one-dimensional array like structure with homogeneous data.

The data can be of any type (integer, string, float, etc.). The axis labels are collectively called index.

For example, the following series is a collection of integers 10, 20, 30, 40, 50, 60, 70, 80, 90, 100.

Key Points of Pandas Series
Homogeneous data

Size of series immutable

Values of data mutable

Series Constructor
A Pandas Series can be created using the following constructor −

pandas. Series (data, index, dtype, copy)

The parameters of the constructor are as follows –

data - data takes various forms like ndarray, list, dictionary, constants, etc.

index- index values must be unique, hashable and have the same length as data. The default index is RangeIndex (0, 1, 2, …, n) if no index is passed.

dtype - dtype is for data type. If none, data type will be inferred.

copy - Copy input data. Default value is False.
**Pandas DataFrame**
A Dataframe is a two-dimensional data structure. So, data is aligned in a tabular fashion in rows and columns. Its column types can be heterogeneous: - that is, of varying types. It is similar to structured arrays in NumPy with mutability added.

Properties of Dataframe are as follows:-
The dataframe is conceptually analogous to a table or spreadsheet of data.

Its columns are of different types – float64, int, bool, and so on.

A Dataframe column is a Series structure.

Its size is mutable – columns can be inserted and deleted.

It has labelled axes (rows and columns).

It can be thought of as a dictionary of Series structures where both the rows and columns are indexed, denoted as index in the case of rows and columns in the case of columns.

It can perform arithmetic operations on rows and columns.

Dataframe Constructor
Dataframe is the most commonly used data structure in pandas.

A pandas Dataframe can be created using the following constructor-

pandas.DataFrame(data, index, columns, dtype, copy)

The constructor accepts many different types of arguments:

Dictionary of 1D ndarrays, lists, dictionaries, or Series structures 

2D NumPy array

Structured or record ndarray

Series structures

Another DataFrame structure 
The parameters description of the constructor is as follows –

-data - data takes various forms like ndarray, series, map, lists, dict, constants and also another DataFrame.

-index- Index or array-like

        Index to use for resulting frame. Will default to RangeIndex if no indexing information part of 
        input data and no index provided
        
-columns- Index or array-like

          Column labels to use for resulting frame. Will default to RangeIndex (0, 1, 2, …, n) if no column labels are  
          provided.
          
          
-dtype - data type of each column

-copy - boolean, default False

        Copy data from inputs. Only affects DataFrame / 2d ndarray input
Dataframe Creation
A pandas Dataframe can be created using various inputs like −

• Lists

• dict

• Series

• Numpy ndarrays

• Another Dataframe

8. Pandas Panel
A panel is a 3D container of data.

The term Panel data is derived from econometrics and is partially responsible for the name pandas − pan(el)-da(ta)-s.

The names for the 3 axes are intended to give some semantic meaning to describing operations involving panel data.

They are −

items − axis 0, each item corresponds to a DataFrame contained inside.

major_axis − axis 1, it is the index (rows) of each of the DataFrames.

minor_axis − axis 2, it is the columns of each of the DataFrames.

9. Data import with Pandas
Pandas input output API provides several functions that can be used to import and export various file formats.

Below is the list of file formats and the corresponding functions to import these file formats.

Flat files - read_csv(), to_csv()

Excel files - read_excel(), ExcelWriter(), to_excel()

JSON files - read_json(), to_json()

HTML tables - read_html(), to_html()

SAS files - read_sas()

SQL files - read_sql(), read_sql_query(), read_sql_table(), to_sql()

STATA files - read_stata(), to_stata()

pickle object - read_pickle(), to_pickle()

HDF5 files - read_hdf(), to_hdf()
