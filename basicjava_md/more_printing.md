# More Printing

Let's get used to printing. Write a program that prints an ATM receipt for Java Bank. An example is below. Your output can look slightly different but try to line up the borders and the margins of the text as much as possible

The borders of the receipt are made up of the dash which is between the `0` and `=` keys. And the `|` pipe character which is above the `[Enter]` key. You create a `|` by holding `[shift]` + `\`.

Your receipt will line up if you use only spaces. Tabs are handled differently by the editor \(Eclipse\) so just use spaces to make it easy on yourself. Eclipse will move the cursor 4 positions when you press `[TAB]`. The tab character will be replaced by 8 spaces when the program executes.

```text

+--------------------------------------+
|      Java Bank ATM Receipt           |
|      Wednesday, December 2, 2015     |
|      ATM Location # 123              |
|                                      |
|                                      |
|      Account Number:      1234567    |
|      Customer:     John Q. Public    |
|      Transaction Type:    Deposit    |
|      Transaction Amount:  $500.00    |
|      Account Balance:   $1,500.00    |
|                                      |
|      Thank you for banking with us   |
|            Have a coffee day         |
|                                      |
+--------------------------------------+
```

