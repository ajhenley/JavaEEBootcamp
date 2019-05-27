# How JSTL Works

The JSP Standard Tag Library \(JSTL\) provides tags for common tasks that need to be performed in JSPs.

The steps you need to follow to implement JSTL are: 1. Add the JAR files to your build path 2. Code the tag lib directive 3. Code the JSTL tag

## Make the JSTL JAR files available

Before you can use JSTL tags within an application, you must make the _jstl-impl.jar_ and _jstl-api.jar_ files available to the application. You can add them to the build path just like you add any other external jar file to the build path in your project. You can retrieve the files from here:

```text
javax.servlet.jsp.jstl-api-1.2.1.jar
```

```text
taglibs-standard-impl-1.2.5.jar
```

## Code the taglib directive

At the top of your JSP page you must code a taglib directive to specify the URI and prefix for the JSTL library. You will mostly use the Core and Formatting libraries shown below:

## The primary JSTL libraries

Your JSP page will look like this:

```markup
<!DOCTYPE html>
<html>
<head>
 <meta charset="utf-8">
 <title>Tag Library Example</title>
 <link rel="stylesheet" href="styles/main.css" type="text/css"/>
</head>
<body>
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<table>
 <tr>
 <th>Name</th>
 <th>Value</th>
 </tr>
 <c:forEach var="c" items="${cookie}"> 
 <tr>
 <td><c:out value='${c.value.name}'/></td>
 <td><c:out value='${c.value.value}'/></td>
 </tr>
 </c:forEach> 
</table>
```

## Tags you can code

```java
for each
for tokens
if statement
choose (replacement for if/else)
```

## How to escape output entered by the user

Escape user-entered data to prevent cross-site scripting attacks where the user attempts to insert JavaScript code into your page to create havoc

Email:

First Name:

Last Name:

Official documentation: [http://docs.oracle.com/javaee/5/jstl/1.1/docs/tlddocs/](http://docs.oracle.com/javaee/5/jstl/1.1/docs/tlddocs/)

