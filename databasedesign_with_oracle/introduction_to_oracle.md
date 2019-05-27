# Introduction to Oracle

## Introduction to Oracle

The Oracle database engine is available in 4 editions: Enterprise Edition \(EE\), Standard Edition \(SE\), Standard Edition One \(SE One\) and Express Edition \(XE\). The last-mentioned is the community edition and is sufficient for the purpose of this course. [http://www.oracle.com/technetwork/indexes/downloads/](http://www.oracle.com/technetwork/indexes/downloads/).

SQL-Developer is an IDE with an Eclipse-like look-and-feel and offers access to the database engine. [http://www.oracle.com/technetwork/developer-tools/sql-developer/overview/](http://www.oracle.com/technetwork/developer-tools/sql-developer/overview/)

In the context of Oracle's application builder APEX \(APplication EXpress\) there is a cloud solution consisting of a database engine plus APEX. [https://apex.oracle.com/](https://apex.oracle.com/). Among a lot of other things it offers an SQL workshop where everybody can execute his own SQL commands for testing purpose. On the other hand APEX can be downloaded separately and installed into any of the above editions with the exception of the Express Edition.

## Working with Oracle: the big picture

Let's talk about how Oracle and Java work together to get data from where it's stored and back to the user. We begin with general concepts you may hear from other books or upcoming assignments.We'll then look into some specific topics in greater detail.

### What is a client/server system?

* A client/server system is the hardware and software components with which you use SQL
* Clients are the PCs or workstations of the system. You do your work on the client
* Servers store the files and databases of the system. They provide services to the clients
* Clients and servers connect through the network which is often the internet
* The server requires a Database Management System \(DBMS\) such as Oracle
* The application software is  installed on the client. It allows the user to interact with the server
* Other Application servers include reporting servers and web application servers

### What is JDBC?

Java Database Connectivity \(JDBC\) is an application programming interface \(API\). It allows you to integrate SQL with Java. Think of JDBC as the communication channel between your Java application and Oracle. The program will request some data, Oracle will fufill that request and the program will receive the result.

### What is a relational database and why do we need one?

A relational database organizes data in tables. Tables contain records \(rows\) and fields \(columns\). Corresponding records are linked through key fields called Primary Keys and Foreign Keys. For example, Managers, Departments and Salary information are stored in different tables. Relationships between the tables permit one to find corresponding records. This allows one to can determine the average salary of the managers of every department.

A database is an organized collection of data. It allows for efficient storage and retrieval of data. Key features of a Database Management System \(DBMS\):

* Minimizes redundancy of data
* Permits sharing among users
* Maintains consistency of data even against simultaneous updates
* Enforces data validity and constraints
* Restricts access as needed
* Permits backup and recovery from data loss

### What is SQL?

SQL \(Structured Query Language\) is a specialized programming language. SQL manages data in a relational database such as Oracle. SQL was developed in the 1970's. It is the standard language of relational databases.

### What does SQL allow me to do?

You can do CRUD \(Create, Read, Update, Delete\) operations to the data inside tables.

### What is a database schema?

The schema is the collection of database objects. Schemas are associated with a particular user or group. Schemas can be used to enforce security constraints on the objects within. Schema objects include tables, fields, relationships, views, indexes, procedures, functions, triggers and sequences. There are multiple schemas in one database.

### Your assignment

You're hired! Now you're a developer at Dalton Used Car Emporium. They keep all their data in an Excel workbook.

* List some reasons why a database would be a better option than Excel \(feel free to use the internet to search for reasons\)
* List the different fields you think you would need for the data
* Organize the fields by the tables you think they would need

