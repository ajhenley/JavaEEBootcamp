# How to check if a customer exists

Sometimes you need to know if a particular record exists in the database. For example, does the customer with an ID of 2 exist?

## How to query the database using JPQL

The JPQL statement below will always return a single number. If the customer does not exist then the query will return 0. Otherwise it will return a count of the number of times the customer does exist. You retrieve the count in the total variable. Compare the value of the variable to determine your next action.

```java
//see if customer exists
TypedQuery<Long> query = 
    em.createQuery("SELECT COUNT(c) FROM DemoCustomer c WHERE c.customerId = 2L", Long.class);
long total = query.getSingleResult();
if (total>0)
{
    out.printf("%s", "Customer exists");
}else{
    out.printf("%s", "Customer does not exist");
}
```

