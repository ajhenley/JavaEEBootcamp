# What is JPQL?

The Java Persistence Query Language \(JPQL\) is the query language defined by JPA. JPQL is like SQL.

## How is JPQL different from SQL?

JPQL operates on objects, attributes and relationships. SQL operates on tables and columns. JPQL can read \(SELECT\), as well as update \(UPDATE\) and delete \(DELETE\). In this course you will create dynamic queries using `EntityManager.createQuery()`.

JPQL defines queries for entities \(your classes\) and their persistent state \(the database tables\). The query language allows you to write queries that work for any database. An application that uses JPQL and Oracle does not have to change if the database changes to Microsoft SQL Server.

## Creating Queries Using the Java Persistence Query Language

Select queries read objects from the database. They return a single object or data element, a list of objects or data elements, or an array of objects and data.

The `EntityManager.createQuery()` method queries the database using Java Persistence query language syntax.

## Some example JPQL queries in a Java application

```java
// Query to return a List of employee objects.
Query query = em.createQuery("Select e FROM Employee e WHERE e.salary > 100000");
List<Employee> employees = query.getResultList();

// Query for a single object using a named parameter. The result is a single value.
// The named parameter is set using the query.setParameter() method.
Query query = em.createQuery("Select e FROM Employee e WHERE e.id = :id");
query.setParameter("id", id);
Employee result2 = (Employee)query.getSingleResult();

// Query for a single data element. The result is a single value.
Query query = em.createQuery("Select MAX(e.salary) FROM Employee e");
BigDecimal result3 = (BigDecimal)query.getSingleResult();

// Query for a List of data elements. The result is a List of Strings
Query query = em.createQuery("Select e.firstName FROM Employee e");
List<String> result4 = query.getResultList();

// Query for a List of element arrays. The result is a list of arrays.
Query query = em.createQuery("Select e.firstName, e.lastName FROM Employee e");
List<Object[]> result5 = query.getResultList();
```

## Positional Parameters in Queries

JPA defines named parameters and positional parameters. Named parameters can be specified in JPQL using the syntax :. Positional parameters can be specified in JPQL using the syntax ? or ?. Positional parameters start at position 1 not 0.

## Named parameter query example

```java
Query query = em.createQuery("SELECT e FROM Employee e WHERE e.firstName = :first and e.lastName = :last");
query.setParameter("first", "Bob");
query.setParameter("last", "Smith");
List<Employee> list = query.getResultList();
```

## Positional parameter query example

```java
Query query = em.createQuery("SELECT e FROM Employee e WHERE e.firstName = ? and e.lastName = ?");
query.setParameter(1, "Bob");
query.setParameter(2, "Smith");
List<Employee> list = query.getResultList();
```

## JPA Query with wildcards

What we are trying to do is get all the items that matches a pattern anywhere in their name.

The SQL query looks like this:

```text
SELECT userName FROM Profile p WHERE p.userName LIKE %pattern%;
```

The JPQL query looks like this:

```java
SELECT p FROM Profile p WHERE p.userName LIKE ?1
```

In your program this looks like this:

```text
String pattern = "Smi%";
Query query = em.createQuery("SELECT p FROM Profile p WHERE p.userName LIKE ?1");
query.setParameter(2, pattern);
List<Employee> list = query.getResultList();
```

