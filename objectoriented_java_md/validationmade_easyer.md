# Validation made Easy - er

As users input data into your program you suddenly find the need to validate it. After all, if your program is expecting a numeric quantity it wouldn't do to have the user enter a negative number or a 'Q'. That's where validation comes in. You can create your own validation class and display an error message to the user if their input is not valid. We'll want to be sure the user can only enter strings, doubles or integers.

We'll look at two ways to validate incoming data

* Use the Scanner class to ensure you only get a particular type of data
* Write your own class to validate that the data is within a specific range

## Using the Scanner class

Here's an example where we use the Scanner class to ensure we get valid data from the user.

The Scanner class contains a wealth of features for validating and parsing data. The code below usesthe Scanner's `hasNextInt()` and `hasNextDouble()` methods to determine if the user entered the expected data. We _could_ throw an exception in the else clause but we choose to exit gracefully.

## Writing your own class

We can't extend the Scanner class because it's final. The reason is that Oracle doesn't want users to change the standard Java classes. The keeps Java working as expected. It also provides some security and efficiency benefits. In fact, most of the Java standard class library is final.

## Your assignment

Sometimes the Scanner class alone doesn't enforce all our business rules. Modify the program above. Add and also implement a Validation class that ensures the following:

* The product code must be exactly five characters long
* Quantity is between 0 and 100 
* Price is between 0.0 and 1000.00

