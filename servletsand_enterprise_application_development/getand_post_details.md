# Get and Post Details

The example application below will show you the results of submitting a form via Get and via Post. The index page contains two forms. The only difference between the two forms is one sends its data via get and the other via post. Create this project in Eclipse. Once you run it you will get a better understanding of get and post and the Request object which comes from the browser.

The GET method sends form information via the URL. When using the GET method the 3rd section of the request packet, the request body, remains empty.

The servlet receives form data in the request packet when you create an HTML form and request `method=POST` is part of the tag. The POST method allows the client to send form data to the server in the request body section of the request. The data is encoded and is formatted similar to the GET method. The data is sent to the server through the URL.

Let's see this actually work. Create the following form in a page called index.html.

 Next, Create a servlet and replace both doGet and doPost with the following code

