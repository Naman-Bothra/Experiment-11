# Experiment-11
Experiment 11- Creating and loading Dataset
NAME:Naman Bothra

PRN: 25070123078

**AIM OF THE EXPERIMENT:** To create a dataset and load an existing dataset using Python (Pandas library) and to analyze basic dataset properties such as shape, size, information, and statistical description.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Theory:-**

Introduction to Pandas and Dataset Handling

In data analysis and data science, datasets are used to store structured information that can be processed and analyzed using programming tools. Python provides a powerful library called pandas, which is widely used for data manipulation and analysis.

Pandas provides two main data structures:

1)- Series – One-dimensional labeled array.

2)- DataFrame – Two-dimensional labeled data structure with rows and columns (similar to a table or spreadsheet).

A DataFrame is the most commonly used structure for handling datasets in Pandas. It allows users to store data in tabular format and perform operations such as filtering, sorting, statistical analysis, and exporting data.

--->Function Used: pd.DataFrame()

Syntax: df = pd.DataFrame(data)

Description: Converts structured data such as dictionaries or lists into a DataFrame. Each key becomes a column name. Each value list becomes the column data.

Example

df = pd.DataFrame(data)

This creates a tabular dataset named df.

Saving Dataset to CSV File

--->Function Used: df.to_csv()

Syntax: df.to_csv("filename.csv", index=False)

Description: Converts the DataFrame into a CSV (Comma Separated Values) file.
CSV files are commonly used for storing tabular data and can be opened in software such as Excel. index=False prevents Pandas from writing row index numbers into the file.

--->Function used: df.shape

It returns the dimensions of the dataset.

--->Function used: df.size

It return the total number of elements in the dataset

--->Function used: df.info

This function provides a summary of the DataFrame, including:

Number of entries (rows)

Column names

Number of non-null values

Data types of each column

Memory usage

--->Function used: df.describe

This function generates statistical summary of numerical columns in the dataset.

--->Function used: df.head()

df.head() is a Pandas function used to display the first 5 rows of a DataFrame. It helps users quickly view the structure and contents of the dataset without printing the entire data.

--->Function used: df.tails()

df.tail() is a Pandas function used to display the last few rows of a DataFrame. It helps users quickly view the ending records of the dataset without printing the entire table.

By default, the function returns the last 5 rows of the dataset. You can also specify the number of rows you want to display.

--->Function used: df.columns

df.columns is a Pandas attribute used to display the names of all the columns present in a DataFrame. When used with print(), it outputs the list of column labels in the dataset.

This helps users quickly understand the structure of the dataset and the available variables.

--->Function used: df.sample()

df.sample() is a Pandas function used to display random rows from a DataFrame. It helps in selecting a random sample of data from the dataset.

--->Function used: df.isnull().sum()

df.isnull().sum() is a Pandas operation used to check for missing (null) values in a dataset. It helps identify how many missing values are present in each column of the DataFrame.

--->Function used: df.duplicated().sum()

df.duplicated().sum() is a Pandas operation used to find the number of duplicate rows in a DataFrame.

--->Function used: df.nunique()

df.nunique() is a Pandas function used to count the number of unique (distinct) values in each column of a DataFrame.

It checks every column in the dataset and returns the total number of different values present in that column.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Conclusion**

In this experiment, a dataset was successfully created and analyzed using the Python Pandas library. The dataset was converted into a DataFrame, stored in a CSV file, and various functions were used to explore and understand the data.

Functions such as df.head(), df.tail(), df.shape, df.size, df.columns, df.sample(), df.isnull().sum(), df.duplicated().sum(), df.nunique(), df.info(), and df.describe() were used to examine the dataset structure, detect missing values, identify duplicates, and obtain statistical information.

Thus, the experiment helped in understanding basic data handling, inspection, and analysis techniques using Pandas, which are essential for data analysis and data science applications.
