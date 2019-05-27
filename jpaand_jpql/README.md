# JPA and JPQL

> JPA stands for Java Persistence API  
>  JPQL stands for Java Persistence Query Language

The Java Persistence API \(JPA\) is a Java specification for accessing, persisting, and managing data between Java objects \(classes\) and a relational database.

> JPA is considered the standard industry approach for Object to Relational Mapping \(ORM\).

JPA itself is just a specification, not a product; it cannot perform persistence or anything else by itself. JPA is a set of interfaces, and requires an implementation. There are open-source and commercial JPA implementations. JPA also requires a database.

JPA allows POJO \(Plain Old Java Objects\) to be persisted. They don't need any interfaces or methods. The object's object-relational mappings are defined through standard annotations or XML. This defines how the Java class maps to a relational database table. JPA also defines a runtime EntityManager API. This is for processing queries and transactions on the objects against the database. JPA defines an object-level query language, JPQL. JPQL allows querying of the objects from the database.

