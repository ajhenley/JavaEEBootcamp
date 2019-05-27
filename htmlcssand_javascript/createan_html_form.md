# Create an HTML Form

The `<form> ... </form>` tag creates an HTML form which will accept user input. It requireds two attributes: action and method. The action attribute tells the form the url of the JSP or servlet that can receive it's data. The method attribute tells the form to send the data via either 'get' or 'post'. Get sends data as appended names and values in the url. Post sends data as part of the request object that goes back to the server. A compete, simple form that sends it's data to a servlet called ProcessForm looks like this:

```markup
<form action="ProcessForm" method="post"/>
<input type="text" name="username">
<input type="password" name="userpassword"/>
<input type="submit" value="Submit"/>
</form>
```

When the servlet processes this form it will receive the data in the format:

```markup
username=dave&userpassword=blue123
```

The `<form&gt;` element can contain one or more of the form elements shown below. Every form element that passes data must contain a name attribute.

```markup
<input>
<textarea>
<button>
<select>
<option>
<optgroup>
<fieldset>
<label>
```

## Your Assignment

Create a web page with an html login form. The form should contain two text boxes. One for user name and one for password. Also allow the user to specify their favorite color. And, of course, include a submit button.

The action will be blank so it won't do anything. The form method should be 'post'. We'll talk about the action later once we set up a JSP or Servlet to receive the data.

Add a link from one of your other pages to go to the form page.Add a link to the form page to go back to one of your other pages.

