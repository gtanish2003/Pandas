
# Pandas Series

A Pandas Series is like a column in a table, representing a 1-D array holding data of any type.

## Series Attributes

### `dtype`
- **Description:** Returns the data type of the elements in the Series.
- **Syntax:** `series.dtype`

### `size`
- **Description:** Returns the number of elements in the Series.
- **Syntax:** `series.size`

### `name`
- **Description:** Returns or sets the name of the Series.
- **Syntax:** `series.name`

### `is_unique`
- **Description:** Checks if all elements in the Series are unique.
- **Syntax:** `series.is_unique`

### `index`
- **Description:** Returns the index of the Series.
- **Syntax:** `series.index`

### `values`
- **Description:** Returns the data as a NumPy array.
- **Syntax:** `series.values`

### `type`
- **Description:** Returns the type of the Series (always `pandas.core.series.Series`).
- **Syntax:** `type(series)`

## Series Methods

### `head`
- **Description:** Returns the first n elements of the Series.
- **Syntax:** `series.head(n)`

### `tail`
- **Description:** Returns the last n elements of the Series.
- **Syntax:** `series.tail(n)`

### `len`
- **Description:** Returns the number of elements in the Series.
- **Syntax:** `len(series)`

### `sample`
- **Description:** Returns a random sample of items from the Series.
- **Syntax:** `series.sample(n, random_state=None)`

### `value_counts`
- **Description:** Returns a Series containing counts of unique values.
- **Syntax:** `series.value_counts()`

### `sort_values`
- **Description:** Sorts the Series by values.
- **Syntax:** `series.sort_values(ascending=True)`

### `sort_index`
- **Description:** Sorts the Series by index.
- **Syntax:** `series.sort_index(ascending=True)`

## Series Math Methods

### `count`
- **Description:** Returns the number of non-null elements in the Series.
- **Syntax:** `series.count()`

### `sum`
- **Description:** Returns the sum of all elements in the Series.
- **Syntax:** `series.sum()`

### `product`
- **Description:** Returns the product of all elements in the Series.
- **Syntax:** `series.product()`

### `mean`
- **Description:** Returns the mean of the Series.
- **Syntax:** `series.mean()`

### `mode`
- **Description:** Returns the mode(s) of the Series.
- **Syntax:** `series.mode()`

### `median`
- **Description:** Returns the median of the Series.
- **Syntax:** `series.median()`

### `std`
- **Description:** Returns the standard deviation of the Series.
- **Syntax:** `series.std()`

### `var`
- **Description:** Returns the variance of the Series.
- **Syntax:** `series.var()`

### `min`
- **Description:** Returns the minimum value in the Series.
- **Syntax:** `series.min()`

### `max`
- **Description:** Returns the maximum value in the Series.
- **Syntax:** `series.max()`

### `describe`
- **Description:** Generates descriptive statistics of the Series.
- **Syntax:** `series.describe()`

# Pandas Series Methods

## `astype`
- **Description:** Casts the Series to a specified dtype.
- **Syntax:** `series.astype(dtype)`

## `between`
- **Description:** Returns a boolean Series indicating whether each element is between two given values.
- **Syntax:** `series.between(left, right, inclusive=True)`

## `clip`
- **Description:** Limits the values in the Series to be within an interval.
- **Syntax:** `series.clip(lower=None, upper=None)`

## `drop_duplicates`
- **Description:** Returns a Series with duplicate values removed.
- **Syntax:** `series.drop_duplicates()`

## `isnull`
- **Description:** Returns a boolean Series indicating which elements are null (NaN).
- **Syntax:** `series.isnull()`

## `dropna`
- **Description:** Returns a Series with null (NaN) values dropped.
- **Syntax:** `series.dropna()`

## `fillna`
- **Description:** Fills null (NaN) values with a specified value or method.
- **Syntax:** `series.fillna(value=None, method=None)`

## `isin`
- **Description:** Returns a boolean Series indicating whether each element is contained in a specified list.
- **Syntax:** `series.isin(values)`

## `apply`
- **Description:** Applies a function to each element in the Series.
- **Syntax:** `series.apply(func)`

## `copy`
- **Description:** Returns a copy of the Series.
- **Syntax:** `series.copy()`


# Pandas DataFrame

## DataFrame Attributes and Methods

### `shape`
- **Description:** Returns the dimensions (rows, columns) of the DataFrame.
- **Syntax:** `dataframe.shape`

### `dtype`
- **Description:** Returns the data type of each column in the DataFrame.
- **Syntax:** `dataframe.dtypes`

### `index`
- **Description:** Returns the index (row labels) of the DataFrame.
- **Syntax:** `dataframe.index`

### `columns`
- **Description:** Returns the column labels of the DataFrame.
- **Syntax:** `dataframe.columns`

### `values`
- **Description:** Returns the data as a NumPy array.
- **Syntax:** `dataframe.values`

### `head`
- **Description:** Returns the first n rows of the DataFrame.
- **Syntax:** `dataframe.head(n)`

### `tail`
- **Description:** Returns the last n rows of the DataFrame.
- **Syntax:** `dataframe.tail(n)`

### `sample`
- **Description:** Returns a random sample of rows from the DataFrame.
- **Syntax:** `dataframe.sample(n, random_state=None)`

### `info`
- **Description:** Prints a concise summary of the DataFrame's information.
- **Syntax:** `dataframe.info()`

### `describe`
- **Description:** Generates descriptive statistics of the DataFrame.
- **Syntax:** `dataframe.describe()`

### `isnull`
- **Description:** Returns a DataFrame of the same shape as the input indicating whether each element is null (NaN).
- **Syntax:** `dataframe.isnull()`

### `isnull().sum()`
- **Description:** Returns the count of null values for each column.
- **Syntax:** `dataframe.isnull().sum()`

### `duplicated`
- **Description:** Returns a boolean Series indicating whether each row is a duplicate.
- **Syntax:** `dataframe.duplicated()`

### `duplicated().sum()`
- **Description:** Returns the count of duplicate rows.
- **Syntax:** `dataframe.duplicated().sum()`

### `rename`
- **Description:** Renames the columns or index of the DataFrame.
- **Syntax:** `dataframe.rename(columns={'old_name': 'new_name'}, index={'old_index': 'new_index'})`

## Mathematical Methods

### `sum`
- **Description:** Returns the sum of values for each column.
- **Syntax:** `dataframe.sum()`

### `min`
- **Description:** Returns the minimum value for each column.
- **Syntax:** `dataframe.min()`

### `max`
- **Description:** Returns the maximum value for each column.
- **Syntax:** `dataframe.max()`

### `mean`
- **Description:** Returns the mean value for each column.
- **Syntax:** `dataframe.mean()`

### `median`
- **Description:** Returns the median value for each column.
- **Syntax:** `dataframe.median()`

### `mode`
- **Description:** Returns the mode(s) for each column.
- **Syntax:** `dataframe.mode()`

### `count`
- **Description:** Returns the number of non-null values for each column.
- **Syntax:** `dataframe.count()`

### `std`
- **Description:** Returns the standard deviation for each column.
- **Syntax:** `dataframe.std()`

### `var`
- **Description:** Returns the variance for each column.
- **Syntax:** `dataframe.var()`

## Selecting Columns from a DataFrame

### `dataframe['column_name']`
- **Description:** Selects a single column from the DataFrame.
- **Syntax:** `dataframe['column_name']`

### `dataframe[['col1', 'col2']]`
- **Description:** Selects multiple columns from the DataFrame.
- **Syntax:** `dataframe[['col1', 'col2']]`

## Selecting Rows from a DataFrame

### `dataframe[start:stop]`
- **Description:** Selects rows by index from start to stop-1.
- **Syntax:** `dataframe[start:stop]`

### `dataframe.loc[label]`
- **Description:** Selects a row by label using the index.
- **Syntax:** `dataframe.loc[label]`

### `dataframe.iloc[index]`
- **Description:** Selects a row by integer location.
- **Syntax:** `dataframe.iloc[index]`

## Fancy Indexing

- **Description:** Uses boolean arrays or masks for advanced indexing.
- **Syntax:** `dataframe[boolean_condition]`

## Selecting Both Rows and Columns

### `dataframe.loc[rows, columns]`
- **Description:** Selects specific rows and columns using labels.
- **Syntax:** `dataframe.loc[rows, columns]`

### `dataframe.iloc[rows, columns]`
- **Description:** Selects specific rows and columns using integer locations.
- **Syntax:** `dataframe.iloc[rows, columns]`

## Filtering a DataFrame

### `dataframe[dataframe['column'] > condition]`
- **Description:** Filters rows based on a specified condition.
- **Syntax:** `dataframe[dataframe['column'] > condition]`

## Adding New Column

### `dataframe['new_column'] = values`
- **Description:** Adds a new column with specified values.
- **Syntax:** `dataframe['new_column'] = values`

# Functions in DataFrame

## More Important Functions

### `value_counts`

- **Description:** Returns a Series with counts of unique values.
- **Syntax:** `dataframe['column'].value_counts()`

### `sort_values`

- **Description:** Sorts the DataFrame by specified column(s).
- **Syntax:** `dataframe.sort_values(by=['col1', 'col2'], ascending=[True, False])`

### `rank`

- **Description:** Assigns ranks to data, with ties getting the average of ranks.
- **Syntax:** `dataframe['column'].rank()`

### `sort_index`

- **Description:** Sorts the DataFrame by index.
- **Syntax:** `dataframe.sort_index(ascending=True)`

### `set_index`

- **Description:** Sets the DataFrame index using existing columns.
- **Syntax:** `dataframe.set_index('column')`

### `rename`

- **Description:** Renames the columns or index of the DataFrame.
- **Syntax:** `dataframe.rename(columns={'old_name': 'new_name'}, index={'old_index': 'new_index'})`

### `reset_index`

- **Description:** Resets the DataFrame index.
- **Syntax:** `dataframe.reset_index()`

### `unique & nunique`

- **Description:** Returns unique values or counts of unique values.
- **Syntax:** `dataframe['column'].unique()` or `dataframe['column'].nunique()`

### `isnull/notnull/hasnans`

- **Description:** Returns boolean Series indicating null values.
- **Syntax:** `dataframe.isnull()`, `dataframe.notnull()`, `dataframe.hasnans`

### `dropna`

- **Description:** Removes null values from the DataFrame.
- **Syntax:** `dataframe.dropna()`

### `fillna`

- **Description:** Fills null values with specified value or method.
- **Syntax:** `dataframe.fillna(value=None, method=None)`

### Two More Attributes: `ffill` and `bfill`

- **Description:** Forward-fill (propagate previous value) or backward-fill (propagate next value) null values.
- **Syntax:** `dataframe.ffill()`, `dataframe.bfill()`

### `drop_duplicates`

- **Description:** Removes duplicate rows from the DataFrame.
- **Syntax:** `dataframe.drop_duplicates()`

### `drop`

- **Description:** Drops specified columns or rows from the DataFrame.
- **Syntax:** `dataframe.drop(columns=['col1', 'col2'])`, `dataframe.drop(index=[1, 2])`

### `apply`

- **Description:** Applies a function along the axis of the DataFrame.
- **Syntax:** `dataframe.apply(func, axis=0)`

### `isin`

- **Description:** Returns boolean DataFrame indicating whether elements are in specified values.
- **Syntax:** `dataframe.isin(values)`

### `corr`

- **Description:** Computes pairwise correlation of columns.
- **Syntax:** `dataframe.corr()`

### `nlargest/nsmallest`

- **Description:** Returns the largest/smallest values in a column.
- **Syntax:** `dataframe['column'].nlargest(n)`, `dataframe['column'].nsmallest(n)`

### `insert`

- **Description:** Inserts a new column at a specified location.
- **Syntax:** `dataframe.insert(loc, column, value)`

### `copy`

- **Description:** Creates a copy of the DataFrame.
- **Syntax:** `dataframe.copy()`


# Merging of DataFrames

## Pandas Data Manipulation

### `pd.concat`

- **Description:** Concatenates two or more DataFrames along rows or columns.
- **Syntax:** `pd.concat([df1, df2], axis=0)` (Concatenating along rows), `pd.concat([df1, df2], axis=1)` (Concatenating along columns)

### `df.append` (Deprecated)

- **Description:** Appends rows of a DataFrame to another DataFrame.
- **Syntax:** `df1.append(df2)`

## Merge Operations

### `merge`

- **Description:** Combines two DataFrames based on a common column using a database-style join.
- **Syntax:** `pd.merge(left, right, on='common_column', how='inner')`

### Merge Variants

- **`left`:** Left outer join (keeps all rows from the left DataFrame).
  - **Syntax:** `pd.merge(left, right, on='common_column', how='left')`

- **`right`:** Right outer join (keeps all rows from the right DataFrame).
  - **Syntax:** `pd.merge(left, right, on='common_column', how='right')`

- **`outer`:** Full outer join (keeps all rows from both DataFrames).
  - **Syntax:** `pd.merge(left, right, on='common_column', how='outer')`

- **`self` or `inner`:** Inner join (keeps only the common rows from both DataFrames).
  - **Syntax:** `pd.merge(left, right, on='common_column', how='inner')`

- **`full` or `outer`:** Full outer join (keeps all rows from both DataFrames).
  - **Syntax:** `pd.merge(left, right, on='common_column', how='outer')`


# GroupBy in Pandas 
The GroupBy functionality in Pandas is a powerful tool for splitting a DataFrame into groups based on a specified criterion and then applying various aggregate functions to these groups. This README provides detailed information on each function associated with GroupBy in Pandas.

**Syntax**
```python

# GroupBy syntax
dataframe.groupby('column_name')
```

# 1. sum()
Calculates the sum of the numeric values in each group.
```python
# Syntax for sum()
grouped_data.sum()
```

# 2. mean()
Calculates the mean of the numeric values in each group.
```python
# Syntax for mean()
grouped_data.mean()
```

# 3. min()
Finds the minimum value in each group.
```python
# Syntax for min()
grouped_data.min()
```

# 4. max()
Finds the maximum value in each group.
```python
# Syntax for max()
grouped_data.max()
```

# 5. size()
Returns the number of items in each group.
```python
# Syntax for size()
grouped_data.size()
```

# 6. first()
Returns the first item in each group.
```python
# Syntax for first()
grouped_data.first()
```

# 7. last()
Returns the last item in each group.
```python
# Syntax for last()
grouped_data.last()
```

# 8. nth()
Returns the nth item in each group.
```python
# Syntax for nth()
grouped_data.nth(n)
```

# 9. get_group()
Gets all items of a specific group.
```python
# Syntax for get_group()
grouped_data.get_group('group_key')
```

# 10. groups
Returns a dictionary with group labels as keys and corresponding indices as values.
```python
# Syntax for groups
grouped_data.groups
```

# 11. describe()
Generates descriptive statistics for each group.
```python
# Syntax for describe()
grouped_data.describe()
```

# 12. sample()
Returns a random sample from each group.
```python
# Syntax for sample()
grouped_data.sample()
```

# 13. nunique()
Returns the number of unique values in each group.
```python
# Syntax for nunique()
grouped_data.nunique()
```

# 14. agg()
Applies a list of aggregation functions to each group.
```python
# Syntax for agg()
grouped_data.agg(['sum', 'min', 'max'])
```

# 15. apply()
Applies a function to each group.
```python
# Syntax for apply()
grouped_data.apply(func)
```

# 16. Multiple Columns GroupBy
```python
# Syntax for GroupBy on multiple columns
dataframe.groupby(['column1', 'column2'])
``` 

# Multilevel Indexing or Hierarchical Indexing

## How to create a multi-indexed object

# 1. pd.MultiIndex.from_tuples()
Creates a MultiIndex from a list of tuples.
```python
pd.MultiIndex.from_tuples([(level1_val1, level2_val1), (level1_val2, level2_val2), ...])
```

# 2.pd.MultiIndex.from_product()
Creates a MultiIndex from the Cartesian product of iterables.
```python
pd.MultiIndex.from_product([level1_values, level2_values, ...])
```

# 3. Creating a series with MultiIndex object
MultiIndex is used to convert higher-dimensional data to lower-dimensional data.
```python

s = pd.Series([1, 2, 3, 4, 5, 6, 7, 8], index=multiindex)
```

# 4. Unstacking and Stacking
## 4.1. unstack
Converts a MultiIndex series to a DataFrame.
```python
s_unstacked = s.unstack()
```

## 4.2. stack
Reverses the operation of unstack.
```python
s_stacked = s.unstack().stack()
```

# 5. sort_index
Sorts the MultiIndex.
```python
s_sorted = s.sort_index()
```

# 6. swap_level
Swaps levels of the MultiIndex.
```python
s_swapped = s.swaplevel()
```

# 7.transpose
Transposes the MultiIndex series.
```python
s_transposed = s.transpose()
```

# 8. Data Formats
## 8.1. Long Data Format: 
Represents each data point with multiple rows, each containing the value of a particular attribute for a given data point.
## 8.2. Wide Data Format:
 Represents each data point with a single row, and multiple columns hold the values of various attributes.


```python

long_data = pd.melt(dataframe, id_vars=['id'], var_name='attribute', value_name='value')
Converts wide-format data to long-format data.
```
# Pivot Table
Creates a pivot table summarizing the data.
It is reverse of melt.
```python
pivot_table = dataframe.pivot_table(index='index_column', columns='columns_column', values='values_column', aggfunc='agg_function', margins=True, fill_value='fill_value')
```

# String Vectorization Operations in Pandas

In data manipulation using Pandas, string vectorization operations can be applied to efficiently transform text data in a DataFrame column. The following common string operations can be performed using the `str` accessor:

1. **Lowercase Conversion (`str.lower()`):**
    ```python
    df['ColumnName'].str.lower()
    ```
   Converts all strings in the specified column to lowercase.

2. **Uppercase Conversion (`str.upper()`):**
    ```python
    df['ColumnName'].str.upper()
    ```
   Converts all strings in the specified column to uppercase.

3. **Capitalize First Letter (`str.capitalize()`):**
    ```python
    df['ColumnName'].str.capitalize()
    ```
   Capitalizes the first letter of each string in the specified column.

4. **Title Case Conversion (`str.title()`):**
    ```python
    df['ColumnName'].str.title()
    ```
   Converts each word in the specified column to title case (capitalizes the first letter of each word).

5. **Stripping Whitespace (`str.strip()`):**
    ```python
    df['ColumnName'].str.strip()
    ```
   Removes leading and trailing whitespaces from each string in the specified column.

6. **Splitting Strings (`str.split()`):**
    ```python
    df['ColumnName'].str.split()
    ```
   Splits each string in the specified column into a list of substrings.

    - Parameters:
        - `n`: (Optional) Number of splits. Default is all occurrences.
        - `expand`: (Optional) If True, return DataFrame with each split as a separate column.

7. **String Replacement (`str.replace()`):**
    ```python
    df['ColumnName'].str.replace('old', 'new')
    ```
   Replaces occurrences of a specified substring in each string of the specified column.

8. **Starts with (`str.startswith()`):**
    ```python
    df['ColumnName'].str.startswith('prefix')
    ```
   Returns a boolean Series indicating whether each string in the specified column starts with the specified prefix.

9. **Ends with (`str.endswith()`):**
    ```python
    df['ColumnName'].str.endswith('suffix')
    ```
   Returns a boolean Series indicating whether each string in the specified column ends with the specified suffix.

10. **Is Digit (`str.isdigit()`):**
    ```python
    df['ColumnName'].str.isdigit()
    ```
   Returns a boolean Series indicating whether each string in the specified column consists of digits only.

11. **Is Alpha (`str.isalpha()`):**
    ```python
    df['ColumnName'].str.isalpha()
    ```
   Returns a boolean Series indicating whether each string in the specified column consists of alphabetic characters only.

12. **Is Alphanumeric (`str.isalnum()`):**
    ```python
    df['ColumnName'].str.isalnum()
    ```
   Returns a boolean Series indicating whether each string in the specified column consists of alphanumeric characters only.

13. **Contains (`str.contains()`):**
    ```python
    df['ColumnName'].str.contains('substring')
    ```
   Returns a boolean Series indicating whether each string in the specified column contains the specified substring.

### General Approach
To perform string vectorization operations in Pandas, use the `str` accessor with the desired operation:
```python
df['ColumnName'].str.string_operation()
```


# Date and Time Operations in Pandas
1. **Creating a Pandas Timestamp**

#### Pandas Timestamp
Pandas `Timestamp` is a data type for representing points in time.
Comparison Between Pandas Timestamp and Python Datetime.
Pandas Timestamp offers additional features and is optimized for time series data.
```python
from datetime import datetime
timestamp = pd.Timestamp('2023-01-01 12:00:00')
```


2. **Using Pandas Timestamp**
```python
ts_pandas = pd.Timestamp('2023-01-01 12:00:00')
```
3. **Using Python datetime**

```python
dt_python = datetime(2023, 1, 1, 12, 0, 0)
```
4. **Creating a DateTimeIndex**

Pandas DateTimeIndex is used for time-based indexing.

```python
date_range = pd.date_range(start='2023-01-01', end='2023-01-10', freq='D')
df = pd.DataFrame({'values': range(10)}, index=date_range)
```
5. **Creating a Date Range**

The date_range function generates a fixed frequency of dates.

```python
date_range = pd.date_range(start='2023-01-01', end='2023-01-10', freq='D')
```
6. **Using to_datetime**


The to_datetime function converts the argument to datetime.

```python
date_str = '2023-01-01'
date_dt = pd.to_datetime(date_str)
```
7. **Accessing datetime properties**

The .dt accessor allows convenient access to the datetime properties.
```python
df['Year'] = df.index.year
df['Month'] = df.index.month
df['Day'] = df.index.day

```
8. **Using errors='coerce'**

The errors='coerce' parameter in functions like pd.to_datetime replaces parsing errors with NaT (Not a Time).
```python
date_str = '2023-01-01xyz'
date_dt = pd.to_datetime(date_str, errors='coerce')
```




















