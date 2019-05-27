# What is a Database?

A database is a program that stores data. There are many types of databases: flat-file, hierarchical, relational, object-relational, object-oriented, xml, and others. The original databases were mainly proprietary and non-standardized.

Relational databases were the first databases to achieve great success and standardization. Relational databases are characterized by the SQL \(structured query language\) standard to query and modify the database, their client/server architecture, and relational table storage structure. Relational databases achieved great success because their standardization allowed many different vendors such as Oracle, IBM, and Sybase to produce interoperable products giving users the flexibility to switch their vendor and avoid vendor lock-in to a proprietary solution. Their client/server architecture allows the client programming language to be decoupled from the server, allowing the database server to support interface APIs into multiple different programming languages and clients.

Although relational databases are relatively old technology, they still dominate the industry. There have been many attempts to replace the relational model, first with object-oriented databases, then with object-relational databases, and finally with XML databases, but none of the new database models achieved much success and relational databases remain the overwhelmingly dominant database model.

The main relational databases used today are: Oracle, MySQL \(Oracle\), PostgreSQL, DB2 \(IBM\), SQL Server \(Microsoft\).

A database management system \(DBMS\) guarantees compliance with the ACID paradigm. This compliance means, that in a multi-user environment all changes to data within one transaction are:

* Atomic: all changes take place or none.
* Consistent: changes transform the database from one valid state to another valid state.
* Isolated: transactions of different users working at the same time will not affect each other.
* Durable: the database retains committed changes even if the system crashes afterwards.

