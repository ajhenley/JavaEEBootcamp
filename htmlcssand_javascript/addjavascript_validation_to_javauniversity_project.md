# Add JavaScript validation to JavaUniversity    project

The onSubmit event of a Form tag can stop a form from processing. If onSubmit calls a function that returns false then the form will not be submitted to the Action. To see an example of this concept copy the following code to a new page and run it. If the input equals the word google then the form will be submitted to the action which is the google website. Otherwise the form will not be submitted.

```markup
<script>
function checkRegistration(){
    var form_valid = (document.getElementById('some_input').value == 'google');
    if(!form_valid){
        alert('Given data is incorrect');
        return false;
    }
    return true;
}
</script>
<form onsubmit="return checkRegistration()" method="get" action="http://google.com">
    Write google to go to google..<br/>
    <input type="text" id="some_input" value=""/>
    <input type="submit" value="google it"/>
</form>
```

Add validation to your Java University project from last week to ensure that the user enters something in the email and password fields.

To do this you will implement the function below to validate the email address. Next you will create a function to validate the form. This function should validate both the email address and also the password box. The function should be called from the onSubmit event of the Form tag.

```markup
function validateEmail(email) { 
 // http://stackoverflow.com/a/46181/11236

 var re = /^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
 return re.test(email);
}
```

On your next page, the data entry page, ensure that the user has entered data in every field by creating a function called ValidateForm and calling it from the onSubmit event of the form.

