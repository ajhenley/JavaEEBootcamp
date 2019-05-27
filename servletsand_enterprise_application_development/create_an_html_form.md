# Create an HTML Form

## An HTML5 document looks like this:

Within that document you can create a form to submit data to the web server. The form goes between the  and tags. Our web server is Tomcat. A servlet is a program which extends Tomcat. The servlet gives Tomcat the ability to handle the url in the @WebServlet annotation at the top of your servlet code file.

## The difference between GET and POST

The form can send its data to the servlet via either GET or POST. They are specified as an attribute of the html form tag. Those are your two choices. GET sends the data in the URL. POST sends the data as the body of the request packet. The above application illustrates the difference.

## A proper form contains the following

* An opening Form tag with an action attribute and a method attribute.
* Any number of inputs each of which must have name attributes identifying the name by which request. The request.getParameter\(\) method in the servlet will retrieve the data from each.
* Labels to identify the inputs for the user.
* A submit button which will tell the browser to send the name and value of each input to the servlet for processing. 
* A closing form tag

The hidden input below can helps the servlet determine which form the user submitted. The form below would go in the body of the html page, between the  and tags.

## Your assignment

* Create a Dynamic Web Project which contains an HTML form to subscribe to your Java Tips email newsletter. 
* You have several email newsletters on your site. They all use the same subscription database. Add a hidden input to pass the name of the newsletter for this form.

