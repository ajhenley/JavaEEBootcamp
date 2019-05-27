# Putting a Basic HTML Page Together

This is the complete page for the Junk Car Emporium example. It may not look great but it works. Upcoming assignments will show you how to add to it.

```text
{%ace edit=true, lang='html'%} 
<html>
<head>
  <title>Dalton Used Car Emporium</title>
</head>
<body>
<div id="main">
  <h1>Welcome to Dalton Used Car Emporium</h1> 
  <h2>If you don't want it, we probably do</h2>
  <img src="cash4junk.png" alt="cash for junk">

  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla consequat faucibus dictum. Nam varius urna velit. Ut sollicitudin a magna id varius. Donec felis odio, interdum sit amet nibh ut, porttitor bibendum nunc. Donec placerat, nunc nec varius sagittis, dui dolor ultrices tortor, venenatis tempor turpis velit ut nulla. Suspendisse bibendum congue dolor eget sollicitudin. Integer consectetur non ipsum pretium laoreet. Phasellus faucibus justo neque, a egestas nisl viverra a. Vestibulum dapibus pulvinar leo vel commodo. Sed tincidunt sapien augue, eu rutrum quam imperdiet eu. Phasellus nunc nisi, commodo eget congue eget, rhoncus imperdiet arcu.</p>

  <img src="oldcar1.jpg" alt="old car 1">
  <img src="oldcar2.jpg" alt="old car 2">
  <img src="oldcar3.jpg" alt="old car 3">
  <img src="oldcar4.jpg" alt="old car 4">

</div>
<div>
  <h2>Contact Us</h2>
  <form action="" method="get">
    Name: <input name="name"><br>
    Reason: <select name="reason">
      <option value="question">Question</option>
      <option value="comment">Comment</option>
       <option value="concern">Concern</option></select><br>
    Message: <textarea rows="3" width="20"></textarea><br>
    <input type="hidden" value="contactForm">
    <input type="submit" value="Contact Us">
  </form>
<footer id="foot01">(c)2016 Dalton Enterprises</footer>  
</div>
</body>
</html>
{%endace%}
```

