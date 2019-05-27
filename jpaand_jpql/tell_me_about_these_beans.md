# Tell Me About These Beans

> **Java Bean**: a class that meets the following criteria:
>
> * Instance varibles are private
> * Instance variables are accessed through public getters and setters 
> * The bean class must implement serializable
> * The bean class must contain a no-argument constructor

## Your first Java Bean

The User class in this example is a JavaBean. We use JavaBeans to pass data between servlets and JSP pages.

## Here's the code for the User class:

```java
public class PersonBean implements java.io.Serializable {
    private String name = null;
    public PersonBean(){}
    public String getName(){
        return name;
    }
    public String setName(String value){
        name = value;
    }
```

## Your Assignment

1. Create another JSP page.
2. Create a link in the first JSP page to the new JSP page.
3. Copy the code above. Will it work?
4. Display the other fields in your class.
5. What happens if you remove sessionScope from the attribute?

## Your second Assignment

1. Next, create an object called Address.java. An address contains the following attributes: Street Address, City, State, ZIP.
2. Add the Address class to the User object. The Address class must be a class in the User class. A User HAS An Address.
3. Change your JSP page to display the User's Address.

