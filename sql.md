# SQL

#### What is a database

Database is a organized collection of data. For example a database of a college would be having a collection of data such as Personal records of Students, Students performance history, Teachers data, Financial department data etc..

### What is SQL?

 SQL stands for Structured Query Language, which is a standardised language for interacting with RDBMS (Relational Database Management System). Some of the popular relational database example are: MySQL, Oracle, mariaDB, postgreSQL etc. SQL is used to perform C.R.U.D (Create, Retrieve, Update & Delete) operations on relational databases. SQL can also perform administrative tasks on database such as database security, backup, user management etc. We can create databases and tables inside database using SQL.


#### What is a Query

A Query is a set of instruction given to the database management system, which tells RDBMS what information you would like to get from the database.


## SQL Syntax

A database is a organized collection of data. Data is stored in relational database in form of tables. To create, retrieve, update and delete from relational database, we use SQL queries.

##### Writing SQL queries

   * To get data from table, you need query

       ```SELECT column_name FROM table_name```

   * all caps not required but helps to tell we are using SQL
   * use ```SELECT * FROM table_name``` to select all the table

##### SQL WHERE Clause

TO fetch the specific rows from the table that meets the given condition.

      ```
      SELECT column_name1, column_name2....column_nameN
      FROM   table_name
      WHERE  CONDITION;
      
      ```

##### Filtering and Sorting

  * ```SELECT DISTINCT column_name``` prevents duplicate column values
  * use ```ORDER BY``` to sort results with ABC, alphabetical, ASC/DESC, ascending/descending
  * use ```LIMIT``` to limit the number of rows returned
  * use ```OFFSET``` to specify where to begin counting rows from

##### Inserting Rows

  * The *database schema* describes the structure of each table and datatypes each column contain
  * Use ```INSERT INTO mytable VALUES``` (value_or_expr, another_value_or_expr, …), (value_or_expr_2,        another_value_or_expr_2, …)  * , …;
  * if you are entering incomplete data, specify the columns ```INSERT INTO mytable (column, another_column, …) VALUES```...

##### Updating Rows

   * ```*UPDATE mytable* SET column = value_or_expr, other_column = another_value_or_expr, … WHERE condition;```
   * datatypes must match the ones specified in the schema

##### Deleting Rows

   * ```DELETE FROM mytable WHERE condition; example example: DELETE FROM movies where year < 2005;```
   * if the WHERE condition is left out, the table will be EMPTIED!

##### Creating Tables

   * ```CREATE TABLE IF NOT EXISTS mytable (column DataType TableConstraint DEFAULT default_value, another_column DataType TableConstraint DEFAULT default_value, …);```


