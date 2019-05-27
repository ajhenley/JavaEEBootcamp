# Create a JavaScript version of Zork

JavaScript is the programming language of the browser. You can use it to make your web pages more interactive.

Use the following html and JavaScript code to get started. follow the instructions from the instructor to create a browser-based version of Zork.

```markup
<html>
<head>
<script>
function Zork(){
v = document.getElementById("command").value;

document.getElementById("message").innerHTML = "<b>You said: " + v + "</b>"
document.getElementById("parlor").style.backgroundColor = "blue";
moves = document.getElementById("moves").text
document.getElementById("moves").value + "\\\rYour next move"
}

</script>
</head>
<body>
<h1>welcome to zork</h1>
<table border="1" style="width:400px">
<tr><td border="1" id="parlor">&nbsp;</td><td border="1" id="vault">&nbsp;</td><td border="1" id="diningRoom">&nbsp;</td></tr>
<tr><td></td><td></td><td></td></tr>
<tr><td></td><td></td><td></td></tr>
</table>

<div id="message">

</div>
<form action="javascript:Zork();">
<input type="text" name="command" id="command"></input>
<input type="submit" id="submit" name="submit">
<img src="http://images.clipartpanda.com/death-clipart-tombstone-clipart.gif" alt="Game over. Dude." height="50"></img>
</form>
<h2>your moves:</h2>
<textarea id="moves" rows="6" cols="50">
</textarea>
</body>
</html>
```

