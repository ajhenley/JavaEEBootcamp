# A first look at Expression Language

> Expression Language is a shortcut notation your JSP pages can use to display objects stored in the session.

Create a new dynamic web application that contains a class for a user. You do not have to connect to the database for this example. Simply create a user class and a servlet.

Once you create a user and populate the name and some other values then put that user object in the session.

## How to add the user to the session:

```java
User user = new User(firstName, lastName, email);
session.setAttribute("user", user);
```

Create a JSP page. When the above code executes it will populate the user class and add it to the session. You can display the user on the JSP page using the following code:

```java
Hello ${sessionScope.user.firstName}
```

## What is Expression Language?

The above code fragment is and example of Expression Language. It's a shortcut notation your JSP pages can use to display objects stored in the session. The word `sessionScope` is optional. The woud `user` is the name of the attribute from the servlet. It contains an instance of a User object which is in the session. The word firstName is formed by removing the word 'get' from the getter, `getFirstName()`, and changing the case of the starting letter. It is also the same as the private variable in the User class but it actually comes from the getter.

