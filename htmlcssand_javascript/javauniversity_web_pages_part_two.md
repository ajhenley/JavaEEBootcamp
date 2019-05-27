# Java University Web Pages Part Two

For Java University we're creating a login page, a data entry page and a report page. The data entry page will allow us to enter a single record and when you click submit it will go to the report page.

Login Page will contain a form with an action called process.jsp. The method should be post.  Normally we won't use jsp pages in this manner. We'll use servlets instead. They have more features for handling such requests. However, a JSP allows us to quickly pass the parameters to other pages without a servlet.

```markup
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Insert title here</title>
</head>
<body>
<form action="process.jsp" method="post">
<input type="text" name="user"></input><br/>
<input type="text" name="password"></input><br/>
<input type="submit"></input>
</form>
</body>
</html>
```

## The process.jsp page should look like this:

```markup
<%@ page language="java" contentType="text/html; charset=ISO-8859-1" pageEncoding="ISO-8859-1" %>
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"/>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=ISO-8859-1"><title>Page title here</title></head>
<body>
Welcome, <%= request.getParameter("user")%><br/>
Your password is <%=request.getParameter("password")%>
</body>
</html>
```

Get the process page working then add a link to the data entry page. On the data entry page you will create a form with an `action="report.jsp" method="post"`. That will display the values from your one record. If we wanted to display lots of records we would need a database and a servlet so that comes later.

**Bonus** Display the user's name and current date on the report page.

