# Line item invoice assignment

## Your Assignment

Create an application that allows users to create an invoice. Users should be able to input data the following data:

* Taxable,total
* Item description
* Item cost
* Number of items

Your application will then apply the tax of 6% and print a subtotal of the items and the tax and a grand total of those two amounts. The user should be able to enter as many items as desired.

```text
Enter your Name: 
Enter the Quantity: 2
Enter the Price: 500.00
Do you want to enter another item (y/n)? y
Enter the Quantity: 3
Enter the Price: 300.00
Do you want to enter another item (y/n) n

You invoice is:

Name: Scott Cook
Address: 4 Quicken Way
City, State ZIP: Intuit, WA 12345

Date: July 5, 2015

Description          Quantity   Price   Total
Item 1 Description         1     10.00   10.00
Item 2 Description         1     10.00   10.00
Item 3 Description         1     10.00   10.00
Item 4 Description         1     10.00   10.00
Item 5 Description         1     10.00   10.00
----------------------------------------------
Number of items: 5
Subtotal: 1,900.00
Tax (6%): 114.00
Grand Total: $2,014.00
```

## Notes

* Your completed solution should use multiple classes. Suggested classes include Invoice, Address, LineItem, Report
* Most of your code should **not** be in the main\(\) method. It should be in classes.
* Users should be able to input data until they run out
* The date and numeric values in your invoice should be formatted accordingly.
* The application will print out an invoice of all the data including a subtotal, tax and grand total.

## Bonus:

Add an extra field to the inputs \(untaxable\). This value will be input as either true or false. This will affect whether tax will be charged on that item or not.

## Extra Bonus:

Create a class called AddressDb which returns an address object. Then the user only has to enter the customer number. You saw this technique in the book database assignment now it's your turn to try it.

