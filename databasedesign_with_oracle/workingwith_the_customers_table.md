# Working with the Customers Table

Now you are going to apply knowledge from a number of different projects.

Be sure you've completed the activity **Import Customers Table**. You'll be building on that activity for this one.

This is a paired assignment. You will work in teams like before. One person should "drive" or direct, the other should type.

1. If you don't have one, add a sequence to the Customers table.
2. Create a JDBC application called CustomerApp which contains a class called Customer \(and other classes as needed\). The application prompts the user for a customer last name and returns the matching record, displaying it on the screen like an address label:

```text
Customer Number: 9
Mr. Robert Dupree
4101 Pickens Way
Longview, TX 75601
RobertODupree@einrot.com
Mapping technician at Irving's Sporting Goods
Press (1) to search for another customer or press (2) to Edit the customer's address.
```

1. Write code in your application that updates a record. If the user presses 2 then your application will prompt for the customer's Street, City, State and ZIP code. The application will receive this data and update the database with the new information.
2. Create unit tests to ensure your application works. At least one unit test should allow you to insert a test name and retrieve that same name back.
3. Allow the user to enter a new customer if the person searched for does not exist in the database.

