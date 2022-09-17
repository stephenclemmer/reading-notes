# Introduction to SQL

Relational databases are a two-dimensional representation of data, formatted as a table. SQL is a means for formatting queries to access specific data contained in a database. Its basic syntax is as follows:

SELECT column, another_table_column, …

FROM mytable

INNER JOIN another_table

ON mytable.id = another_table.id

WHERE condition(s)

ORDER BY column, … ASC/DESC

LIMIT num_limit OFFSET num_offset;

![Exercise 1:](./images/SQL%20Bolt%20Exercise%201.png)
![Exercise 2:](./images/SQL%20Bolt%20Exercise%202.png)
![Exercise 3:](./images/SQL%20Bolt%20Exercise%203.png)
![Exercise 4:](./images/SQL%20Bolt%20Exercise%204.png)
![Exercise 5:](./images/SQL%20Bolt%20Exercise%205.png)
![Exercise 6:](./images/SQL%20Bolt%20Exercise%206.png)

**Inserting Rows:**

When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert. In general, each row of data you insert should contain values for every corresponding column in the table. You can insert multiple rows at a time by just listing them sequentially.

**Insert statement with values for all columns**

INSERT INTO mytable

VALUES (value_or_expr, another_value_or_expr, …),

(value_or_expr_2, another_value_or_expr_2, …),

…;

In some cases, if you have incomplete data and the table contains columns that support default values, you can insert rows with only the columns of data you have by specifying them explicitly.

**Insert statement with specific columns**

INSERT INTO mytable

(column, another_column, …)

VALUES (value_or_expr, another_value_or_expr, …),

(value_or_expr_2, another_value_or_expr_2, …),

…;

In these cases, the number of values need to match the number of columns specified. Despite this being a more verbose statement to write, inserting values this way has the benefit of being forward compatible. For example, if you add a new column to the table with a default value, no hardcoded INSERT statements will have to change as a result to accommodate that change.

In addition, you can use mathematical and string expressions with the values that you are inserting.
This can be useful to ensure that all data inserted is formatted a certain way.

**Example Insert statement with expressions**

INSERT INTO boxoffice

(movie_id, rating, sales_in_millions)

VALUES (1, 9.9, 283742034 / 1000000);

![Exercise 13:](./images/SQL%20Bolt%20Exercise%2013.png)

**Updating Rows:**

UPDATE mytable

SET column = value_or_expr,

other_column = another_value_or_expr,

…

WHERE condition;

![Exercise 14:](./images/SQL%20Bolt%20Exercise%2014.png)

**Deleting Rows:**

DELETE FROM mytable

WHERE condition;

![Exercise 15:](./images/SQL%20Bolt%20Exercise%2015.png)

**Creating Tables:**

CREATE TABLE IF NOT EXISTS mytable (

column DataType TableConstraint DEFAULT default_value,

another_column DataType TableConstraint DEFAULT

default_value,

…

);

![Exercise 16:](./images/SQL%20Bolt%20Exercise%2016.png)

**Altering Tables:**

1. Adding Columns:

ALTER TABLE mytable

ADD column DataType OptionalTableConstraint

DEFAULT default_value;

2. Removing Columns:

ALTER TABLE mytable

DROP column_to_be_deleted;

3. Renaming the table:

ALTER TABLE mytable

RENAME TO new_table_name;

![Exercise 17:](./images/SQL%20Bolt%20Exercise%2017.png)

**Deleting Tables:**

DROP TABLE IF EXISTS mytable;

![Exercise 18:](./images/SQL%20Bolt%20Exercise%2018.png)