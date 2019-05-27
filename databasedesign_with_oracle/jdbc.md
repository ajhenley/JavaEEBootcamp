# JDBC

To develop Java applications which access the Oracle database you will need to download the ojdbc6.jar library from Oracle. You'll need to include that library in your eclipse project.

Here is some example code that will work with the virtual machine. Create a new eclipse project called OracleJDBCTestProject. Then create a class called TestOracleJDBC. Copy the following code to that class.

This code will connect to the database and print the username which is "DEMO". It might print an error message in red. You must fix the error before you can continue to work with Oracle and Java. The most common source of errors is the connection string is incorrect. The second most common source of errors is the sql statment is incorrect. We are using a generic sql statement that should work on any Oracle installation.

## What is a connection string?

In the code below the connection string is `jdbc:oracle:thin:demo/demo@localhost:1521:orcl`. The connection string contains parameters. ODBC.jar library will use those parameters to connect with your instance of the Oracle database.

## Did it work?

Did you see the word DEMO in the Eclipse console? Then you now have Eclipse and Oracle correctly configured.

