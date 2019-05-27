# People Finder

**Prerequisite**: Complete the SQL Bonus Practice. You will be using the tables created in that project for this one. You must create a database with multiple tables.

## Your Assignment

1. Create a dynamic web application to search by last name
2. Create a search form that will allow users to enter a name in a text box and find all the matching last names. If the user enters partial text the application finds all last names that contain that text. So Smith will find users named Smith and Smithman. 
3. Create a page to display the user details once that user is found.

> To search for a partial term in SQL use the ```LIKE`` operator with the wildcard character```%\`\`\`. The percent sign will match any number of letters. Note that our installation of Oracle is case-sensitive. So 'smith' will not match 'Smith'.
>
> So to find all users named Smith use the following SQL statement:

```sql
select firstname,lastname from customers where lastname like 'Smith%'
```

## Submit SQL Scripts in GitHub

When submitting database projects to GitHub. include your SQL Scripts. Create a folder in your project. That folder will be uploaded to GitHub. If you need to rebuild your database you have the latest version under source control.

