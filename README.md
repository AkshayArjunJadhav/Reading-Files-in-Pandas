# Reading-Files-in-Pandas
How to read JSON, Excel, text, and CSV files using Pandas
### 1. Reading JSON Files

JSON (JavaScript Object Notation) files are commonly used for storing structured data. Pandas provides the `pd.read_json()` function to read JSON files into a DataFrame.

```python
import pandas as pd

# Read JSON file into DataFrame
df = pd.read_json('data.json')
```

### 2. Reading Excel Files

Excel files are widely used for tabular data storage. Pandas offers the `pd.read_excel()` function to read Excel files into a DataFrame.

```python
# Read Excel file into DataFrame
df = pd.read_excel('data.xlsx')
```

### 3. Reading Text Files

Text files are plain text files containing structured or unstructured data. Pandas allows you to read text files using the `pd.read_csv()` function by specifying the appropriate delimiter and other parameters if needed.

```python
# Read text file into DataFrame
df = pd.read_csv('data.txt', delimiter='\t')
```

### 4. Reading CSV Files

Comma-Separated Values (CSV) files are commonly used for storing tabular data. Pandas provides the `pd.read_csv()` function to read CSV files into a DataFrame.

```python
# Read CSV file into DataFrame
df = pd.read_csv('data.csv')
```

### Additional Parameters

- **Header:** Specify the row number(s) to use as the column names.
- **Index:** Specify the column(s) to use as the index.
- **dtype:** Specify data types for columns.
- **Skiprows:** Skip specified number of rows from the beginning of the file.
- **Nrows:** Read only the specified number of rows.
- **Encoding:** Specify the file encoding (e.g., 'utf-8', 'latin1').

```python
# Example with additional parameters
df = pd.read_csv('data.csv', header=0, index_col='ID', dtype={'Price': float})
```

### Conclusion

Pandas simplifies the process of reading various file formats into DataFrames, allowing for easy manipulation and analysis of data in Python.

Now, you're equipped to efficiently read JSON, Excel, text, and CSV files using Pandas!
