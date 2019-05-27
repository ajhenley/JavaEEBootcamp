# What can JavaScript do?

## JavaScript

JavaScript is a client side scripting language. JavaScript code, like CSS, is part of the page or a separate file. When a browser requests a page that includes JavaScript, the script and HTML return together to the browser. The browser contains a JavaScript engine that processes the JavaScript.

JavaScript and CSS work differently on different browsers. A great resource for checking browser compatibility is `http://browsershots.org`

HTML pages consist of a collection of tags. This hierarchical collection of tags called the DOM \(document object model\). The power of JavaScript is that it can change the DOM in real time.

JavaScript Can't ...

* Read or write files
* Communicate over the network
* Run other programs

## JavaScript can ...

* Change HTML content and attributes by modifying the DOM \(document object model\) of the web page
* Create dynamic menus
* Validate data in a form before it is sent to the server for processing
* Respond to user actions such as mouse clicks and key presses
* Animate elements in a web page
* Change a CSS style sheet that a web page uses
* Sort the data in a table
* Change images when the user rolls the mouse over it
* Prompt the user

### JavaScript Example

In the example below I have added two paragraph tags with their id attribute set. That helps JavaScript identify the tags. Then as the page is loading the web server comes across the script tags which means the web server will execute the code in that script. So it tells JavaScript to set the value of each identified element to the value indicated. The Date\(\) function returns the current date and tinme.

```markup
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Title of the document</title>
</head>

<body>

<p id="greeting"></p>
<p id="date"></p>
<!--JavaScript can set content for your page-->
<script>
    document.getElementById("greeting").innerHTML = "Hello JavaScript";
    document.getElementById("date").innerHTML = Date();
</script>
</body>

</html>
```

