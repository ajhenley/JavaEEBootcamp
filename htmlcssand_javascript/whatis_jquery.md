# What is JQuery?

jQuery is a JavaScript library. jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code. jQuery handles the complexity behind HTML document traversal and manipulation even across multiple browsers. The purpose of jQuery is to make it much easier to use JavaScript on your website. What can you do with jQuery?

* HTML/DOM manipulation
* CSS manipulation
* HTML event methods
* Effects and animations

## Include jQuery in your web page

Add the following script tag within the head section of your web page to include all the jQuery code in your page.

```markup
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.12.2/jquery.min.js"></script>
```

## What is $\( document \).ready\(\)?

A page can't be manipulated safely until the document is "ready." That means the browser is done retrieving the page from the server.

jQuery detects this state of readiness for you. JavaScript code inside a `$( document ).ready()` block will only run once the page Document Object Model \(DOM\) is ready for JavaScript code to execute.

$\(document\).ready\(\) always takes a function argument. This function is called the handler. The handler is the JavaScript function that will execute once the document is ready. That's why you see the function definition between the parenthesis following ready.

## JavaScript Functions

JavaScript functions like the one in $\(document\).ready\(\) above can be defined without a name. Since you're never calling it anywhere you don't need a function name.

JavaScript functions could also be assigned to variables as `var fn = function(param){return param};` you call such a function as `var response = fn("somevalue");`

```markup
// A $( document ).ready() block.
$( document ).ready(function() {
    //inside the body of the function...
    console.log( "ready!" );
});
```

## Playing nice with others: Putting jQuery Into No-Conflict Mode

When you put jQuery into no-conflict mode, you have the option of assigning a new variable name to replace the $ alias.

jQuery uses `$` as a shortcut for jQuery. Thus, if you are using another JavaScript library that uses the $ variable, you can run into conflicts with jQuery.

Avoid `$` conflicts by putting jQuery in no-conflict mode immediately after it is loaded onto the page and before you reference jQuery in your page.

In the example below, the prototype.js library is another framework that also uses the $ as an alias. Both prototype and jQuery are using the $ alias.

To prevent conflicts, add the jQuery library last and assign another variable which jQuery will use to instead of the $. In the example below we use $j as an alias.

```markup
<!-- Putting jQuery into no-conflict mode. -->
<script src="prototype.js"></script>
<script src="jquery.js"></script>
<script>

var $j = jQuery.noConflict();
// $j is now an alias to the jQuery function; creating the new alias is optional.

$j(document).ready(function() {
    $j( "div" ).hide();
});
```

In the code above, the $ will retain its meaning in original library. You'll still be able to use the full function name jQuery as well as the new alias $j in the rest of your application. The new alias can be named anything you'd like: jq, $J, awesomeQuery, etc.

## What can You do with jQuery?

jQuery makes it easy to hide and show a section of your page. Wrap that section in a div tag and use the tag's id attribute to access it. Then show/hide that tag and all the code it contains. We'll try this now by adding a button to control the toggle and wrapping a contact form around some div tags. jQuery also makes it easy to set content. We'll have jQuery

## Show and Hide a Section of Your Page

```markup
<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.2/jquery.min.js"></script>
<script>
$(document).ready(function(){

    $("#hideById").click(function(){
        if ($("#hideme").is(":visible")){
            $("#hideme").hide();
        }else{
            $("#hideme").show();
        }
    });

    $("#hideContactForm").click(function(){
        if ($(".hideByClass").is(":visible")){ 
            $(".hideByClass").hide();
        }else{
            $(".hideByClass").show();
        }
    });

});
</script>
</head>
<body>

<h2>jQuery Example</h2>

<p>This paragraph will not be hidden when you click the button.</p>
<p id="hideme">This paragraph will be hidden when you click the button.</p>
<div class="hideByClass">
Contact Us:<br/>
<form action="" method="post">
Name: <input type="text"/><br/>
<input type="password"/><br/>
<input type="submit" value="Submit"/>
</form>
</div>

<button id="hideById">Click to Show/Hide the Paragraph</button><br/>
<button id="hideContactForm">Click to Show/Hide the Contact Form</button>
</body>
</html>
```

## Add a Function to the Button Click Event

A button on a web page exposes some properties and methods. One of these is the click event.

You can use jQuery to add code to execute when the click event fires. In the example we define a function that contains two lines of code. It sets the html or text of div tag that has an id of results. The first button sets the text value, the second sets the html value. It is not uncommon to see jQuery scripts which accept a function as a parameter.

```markup
$(document).ready(function(){
    $("#btn1").click(function(){
        var testText = $("#test").text();
        $("#results").text(testText);
    });
    $("#btn2").click(function(){
        var testHTML = $("#test").html()
        $("#results").html(testHTML);
    });
});
```

## Get or Set Content

Here's an example where you can get content based on the element id.

```markup
<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.2/jquery.min.js"></script>
<script>
$(document).ready(function(){
    $("#btn1").click(function(){
        var testText = $("#test").text();
        $("#results").text(testText);
    });
    $("#btn2").click(function(){
        var testHTML = $("#test").html()
        $("#results").html(testHTML);
    });
});
</script>
</head>
<body>

<p id="test">This is some <b>bold</b> text in a paragraph.</p>

<button id="btn1">Show Text</button><br/>
<button id="btn2">Show HTML</button><br/>
Show the results:<br/>
<div id="results"></div>
</body>
</html>
```

