# Sessions in Servlets and Web Pages

Session tracking enables you to track a user's data over multiple servlet, JSP or HTML page requests. A session is a series of related requests that come from the same client \(browser\) during a given period. These requests may represent pages that have some meaning as a whole, such as a shopping cart application.

HTTP is a "stateless" protocol. This means each time a browser retrieves a Web page, the browser opens an unrelated connection to the Web server. The server does not keep a record of previous client requests.

There are three ways to remember the data that is passed between servlets and pages even though the requests for each are separate transactions. They are cookies, request paramenters and session variables.

**Cookies**  
A webserver can assign a unique session ID as a cookie to each web client. Subsequent requests from that client can be recognized using the received cookie.

There is a drawback. Sometimes browsers do not support cookies.

**Request Parameters as Hidden Form Fields**  
A web server can send a hidden HTML form field along with a unique session ID as follows:

When the form gets submitted, the input's name and value are part of the GET or POST data. Each time the web browser sends a request back, the session\_id keeps the track of different requests.

This could be an effective to keep track of the session. Clicking on a hypertext link does not result in a form submission. That only happens when the user clicks a button to submit a form.

 **URL Rewriting**  
You can append extra data to the end of each URL. This could identify the session. The server can associate that session identifier with data it has stored about that session.

For example, with `http://mysite.com/index.jsp?sessionid=12345`, the session identifier is attached to the URL as sessionid=12345. This can be accessed by the the web server to identify the client.

URL rewriting is a better way to maintain sessions and works for the browsers when they don't support cookies. The disadvantage is you have generate every URL dynamically to assign a session ID. You can't do this with a static HTML page. Also, the user can easily change the data as it is passed to the servlet.

## The HttpSession Object

Fortunately, the servlet provides the HttpSession Interface. This gives you a way to identify a user across more than one page request or visit to a Web site.

The servlet container uses this interface to create a session between an HTTP client and an HTTP server. The session persists for a specified time period, across more than one connection or page request from the user.

You would get a reference to the HttpSession object by calling the public method `getSession()` of HttpServletRequest, as below:

`HttpSession session = request.getSession();`

You need to call `request.getSession()` before you send any document content to the client.

