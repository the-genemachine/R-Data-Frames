# R Data Frames

Data frames are the primary data structure for storing and manipulating data in R. They are essentially a list of vectors, where each vector is a column and has the same length.

## Characteristics of Data Frames

1. **Columns can be of different types:** A data frame can contain numeric, factor, character, or other types of columns, all within the same structure.
2. **Rows and columns have names:** Each row and column can be named, which helps in indexing and accessing the data.
3. **They are similar to a matrix:** While matrices in R can only have one type of data (e.g., all numeric), data frames can have a mix of data types.

## Creating a Data Frame

You can create a data frame using the `data.frame()` function:

```r
my_data <- data.frame(
  name = c("Alice", "Bob", "Charlie"),
  age = c(25, 30, 35),
  stringsAsFactors = FALSE
)
```

Note: By default, character vectors are converted to factors in a data frame. You can prevent this by setting `stringsAsFactors = FALSE`.

## Accessing Elements

You can access elements in a data frame in multiple ways:

- **By column name:** `my_data$name` or `my_data[["name"]]`
- **By row and column index:** `my_data[1,2]` accesses the element in the first row and second column.

## Useful Functions

- `head(my_data)`: View the first 6 rows.
- `tail(my_data)`: View the last 6 rows.
- `str(my_data)`: Provides a concise summary of the data frame's structure.
- `dim(my_data)`: Returns the dimensions (rows x columns) of the data frame.

## Summary

Data frames are the fundamental data structure for most data manipulation tasks in R. They allow for flexibility in terms of data types, indexing, and manipulation.
