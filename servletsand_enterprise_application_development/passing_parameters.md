# Passing parameters

You've created a website. It contains an html page, index.html, a servlet, ProcessForm.java, and a results page, output.jsp.

Question: How do you get a value from the form to the servlet and to the output page?

Answer: Use either request parameters or session variables.

## Request Parameters

 Enter your name:  

## Getting the form data into the servlet

When the user clicks the submit button the data from the form gets sent to the servlet in the request object. The web server takes care of this. The servlet container, Tomcat, will make the request object available to your servlet. Your input named userName will contain the name that the user typed. The servlet can read that name by using `request.getParameter("userName")`. You probably want to set it to a variable as in   
 `String name = request.getParameter("userName");`  
 Now your servlet can work with it.

## Sending your values from the servlet to the output page

Now you have a variable in your servlet called userName. You want to send that to output.jsp. Simply add a tag to output.jsp that looks like this:  
 `${message}` and replace the message tag in the jsp with the following line of code:  


