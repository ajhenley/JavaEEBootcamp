# Tell me About Expression Language

The Expression Language \(EL\) is a faster/easier way to display parameter values. It is part of the JSP Specification. Expression Language is helpful for web designers. They may have limited Java knowledge yet still have the need to send and receive data from servlets or other Java objects. EL does this by encoding tags in the JSP. It is possible to use scriptlet tags `<%` and`%>` to accomplish the same task but EL simplifies this process.

```markup
Hello, ${param.visitor}
```

Same as

```markup
Hello, <%=request.getParameter("visitor")%>
```

EL offers a clearer way to navigate nested beans. Consider some beans:

If an instance of Person was to be placed onto a request attribute under the name "person", the JSP would have:

Same as.

