# Aggregate Functions

How to call an aggregate function in JPA:

If it returns a scalar \(one row, one column\) use this...

```java
Query query1 = entitymanager.createQuery("Select MAX(e.salary) from Employee e"); 
Double result = (Double) query1.getSingleResult();
```

If it return multiple columns/rows

```java
Query query1 = entitymanager.createQuery("Select OrderID, SUM(total) from Cart c");
Double emplID =(Double) query1.get(0);
Double salary = (Double) query1.get(1);

List<Object[]> results = em.createQuery("SELECT m.name AS name, 
  COUNT(m) AS total FROM Man AS m GROUP BY m.name ORDER BY m.name ASC");

em.getResultList();

for (Object[] result : results)
{
  String name = (String) result[0];
  int count = ((Number) result[1]).intValue();
}
```

