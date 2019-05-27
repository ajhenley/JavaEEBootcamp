# Creating Tables

In previous applications you saved data to your hard drive. Then you opened the file to read it. A database allows you to do the same thing - save data. It also includes software to ensure the integrity of your data. Your application will communicate with the database by sending SQL queries through the data access API. In this course, you'll use the Java ODBC connection library for this. When the database receives the SQL it will process the query and return the results. For now you'll use SQL Developer to submit your queries and receive the results.

## Creating Tables

Remember how we created a book class for our application? Now we need a Book table to store our data. It should allow for the following fields:

* SKU \(stockkeeping unit - can contain numbers, dashes and possibly letters\)
* Book title \(text\)
* Author \(text\)
* Description \(text\)
* Price \(double\)
* IsInStock \(true/false\)

You'll enter the SQL statement in Oracle SQL Developer. The SQL statement starts with CREATE TABLE followed by the table name. Then a set of parenthesis. Within the parenthesis go the fields, separated by commas. Field names may not contain spaces. Follow each field name with a space and the data type. Close the statement with a semi-colon.

### The Primary key

The primary key is an indicator that tells the database which field will uniquely identify each record. This makes the database operate more efficiently. Data in the primary key is most often numeric and must be unique to each record \(row\).

### Indexes

A database index is a data structure. It improves the speed of data retrieval. It allows the database management system to find correct row without searching every row. Oracle creates indexes for primary keys and unique constraints on a table. If you frequently search other fields you can speed up the query by creating an index.

