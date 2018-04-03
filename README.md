# DATA 515A - Homework 2
Homework 2: Procedural Python
In this homework, we’ll work with the same YouTube data that was used in homework 1.

Create a python module (a file with extension ‘.py’) with the following functions:

* (4 points) `create_dataframe` that creates a pandas `DataFrame` with three columns `video_id, category_id, language` (one of  ‘us’, ‘gb’, ‘fr’, ‘de’, ‘ca’) by processing all of the tables in `class.db`. `create_dataframe` has one argument, the path to the database containing the table.
   - Hint: You can use the pandas method `read_sql` as described in this [article](https://www.dataquest.io/blog/python-pandas-databases/) create a pandas `DataFrame` using a SQL `SELECT` statement.
* (3 points) `test_create_dataframe` that takes a pandas `DataFrame` as input and returns `true` if the following conditions hold:
  * The DataFrame contains only the columns `video_id, category_id, language`.
  * The columns `video_id` and `language` could be a key.
  * There are at least 10 rows in the `DataFrame`.
