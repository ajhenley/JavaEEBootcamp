# ArrayList Activity

You have written invoice applications that are limited by the fact that you were using arrays to store the data. Now that you have ArrayLists in your toolbox, you are to write an invoice application that meets the following specifications:

The Output Should Look Like This

```text
Welcome to the invoice application.

Enter product code: java
Enter quantity:     1
Another line item? (y/n): y

Enter product code: jsps
Enter quantity:     2
Another line item? (y/n): n

Code    Description                     Price   Qty     Total
----    -----------                     -----   ---     -----
java    Dalton's Beginning Java         $49.50  1       $59.50
jsp    Dalton's Learn Java Servlets and JSP  $54.50  2       $99.00

                                        Invoice total:  $148.50
```

It must have these classes

| Name | Description |
| :--- | :--- |
| Product | Represents a Product object. |
| ProductDB | Provides a getProduct method that retrieves the Product object for a specified product code. |
| Validator | Provides methods that accept and validate user input. |
| LineItem | Represents an invoice line item, which includes a Product object, a quantity, and a total. |
| Invoice | Represents a single invoice. The line items are stored in an array list. |
| InvoiceApp | Contains the main method for the Invoice application. |

## Invoice Class Information

### Constructor:

* Invoice\(\)

  **Methods:**

* void addItem\(LineItem lineItem\)
* ArrayList getLineItems\(\)
* double getInvoiceTotal\(\)
* String getFormattedTotal\(\)

