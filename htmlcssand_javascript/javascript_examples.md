# JavaScript Examples

## JavaScript is a real language

JavaScript \("JS" for short\) is a full-fledged dynamic programming language. JavaScript provides dynamic interactivity on websites. JavaScript is compact but flexible. Many tools have been written on top of the JavaScript language allowing one to add functionality with minimal effort.

JavaScript may be the most misunderstood programming language in the world. It combines simplicity with power. It is often misused. JavaScript is finding its way into more and more high-profile applications and gaining acceptance.

### Developer Tools

Let's try some JavaScript examples in the browser. You can save these examples to a web page in the body section. Refresh the page after each edit to see your changes.

If you are using Chrome or Firefox you can open the developer tools. From there you can view the console. You may wish to browse to a blank page so type "about:blank" in the address bar.

Do you need information about using the developer tools?

* Chrome: `https://developer.chrome.com/devtools` 
* Firefox: `https://developer.mozilla.org/en-US/docs/Tools`

Type the following in the developer tools console. If you are working from a web page then the JavaScript code needs to be between `<script> ... </script>` tags. The script tags can go inside the body. You'll have to save and refresh the page with every change.

```markup
document.write('hello, world!');
```

Let's start with variables. A variable has a name and contains a value. Use the `var` keyword followed by the name. Do not define a type. JavaScript will determine the type once you give it data. Until then it will be undefined.

```markup
//this is a comment. It will not be executed
var myVar = 5;
document.write(myVar);
document.write("<br/>")
```

JavaScript uses the `+` to concatenate strings.

```markup
var words = "This sentence ends in a";
var moreWords = " preposition.";
var sentence = words + moreWords;
//go to the next line
document.write(sentence + '<br/>');
```

JavaScript needs you to escape quotes inside strings. Use the `\` to escape the single quote. If your string has double-quotes then you don't have to escape a single quote inside of it.

```markup
//using double or single quotes
var s = 'A string that\'s single quoted'
document.write(s);
document.write("<br/>")

s = "A string that's double quoted"
document.write(s);
document.write("<br/>")
```

Since JavaScript strings are objects they have properties and methods you can access. Here is an example of returning the length property or executing the substring method. For documentation about these and other string properties and methods refer to any of the various online sources. I recommend `https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/About`.

```markup
document.write(sentence.length);
document.write("<br/>")
```

Strings also have methods

```markup
document.write(sentence.substring(2,5);
```

### JavaScript Arrays

The JavaScript Array object is a global object that is used in the construction of arrays; which are high-level, list-like objects.

Here's how you declare an array and print the first item:

```markup
var simpsons = ['homer','marge','lisa','bart'];
document.write("<br/>")
document.write(simpsons[0]);
document.write("<br/>")
```

Now sort the array and display it:

```markup
simpsons.sort();
//display the array
for (var i = 0; i < simpsons.length; i++){
    document.write(simpsons[i]);
}
```

The length property of the array returns a count of the number of items it contains. Since arrays are zero-based the last item will have an index value of one less than the length. Access the last item as shown below:

```markup
var last = simpsons[simpsons.length - 1];
document.write(last);//bart
```

In the next example I show you how to use push to add a new item. The opposite of push is pop which will remove it.

```markup
var donnie = simpsons.push('Donnie');
document.write(simpsons);
simpsons.pop();
```

Remove element at a specific index

```markup
delete a[4];
//display the array
for (var i = 0; i < a.length; i++){
    document.write(a[i])
}
```

Just like in many other programming languages, you can populate an array from a for loop.

```markup
var numbers = [];
for (var i = 0; i < 10; i++){
    numbers[i] = i + 1;
}
//display the array
for (var i = 0; i < 10; i++){
    document.write(numbers[i]+"<br/>");
}
```

### JavaScript Functions

JavaScript lets you define your own functions with the keyword, function. It's a good idea to put the function in the head tags to keep things organized.

```markup
function sayAnything(what){
    document.write(what);
}
//call the function
sayAnything("anything");
```

JavaScript allows you to assign a function to a variable so calling the variable is like calling the function.

```markup
var say = saySomething();
```

Sometimes functions are assigned to a the '$' which is a valid character for variable names. JQuery does this as you'll see.

```markup
<input type="text" id="element"></input>
var $ = function (id){
    return document.getElementById(id);
}
```

You can set the value of the element by the function. If the element was a paragraph this function would return a reference to it.

```markup
$("element")
//return an element by id
document.write($("element"));
```

### Decision making in JavaScript

```markup
var a = 7
if (a > 10){
// do something
}else{
// do something else
}
```

## repetition/looping

```markup
for(i=0;i<5;i++){
document.write("this is iteration number " + i + "<br/>");
}
```

```markup
while (c < 10) {
  c += 1;
  // …
}
```

```markup
while (c < 10) {
  c += 1;
  // …
}
```

### Getting input from user

You can read an element with that contains user-entered text as follows: `var text=document.getElementById('input1').value;`

You can display a message or set the text of an element: `document.getElementById("message").innerHTML = "some text";`

You can also prompt the user with an alert. The script below could go into a function to be called on a button click event. 

```markup
<script>
var response = confirm("Are you sure you want to send a payment?");
if (response == true) {
    msg = "Payment sent!";
    //redirect to another page
} else {
    msg = "Payment cancelled!";
    //stay on current page
}
alert (msg);
</script>
```

