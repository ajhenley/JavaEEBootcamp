# Getting and storing user input

The Scanner object allows people to input data. It captures all the input on a standard input \(like the keyboard\) and delivers it to a variable.

A Scanner scans the input by tokens using a delimiter pattern. The default delimiter is a space. This means that scanner assumes that each time it sees a space it is getting ready to start a new input. So if you want to capture an input that should contain spaces \(like a book title, or someone's full name\), you have to use a special command `nextLine`.The scanner reads the input token by token. The resulting tokens may be converted into values of different types using various methods.

## To include the Scanner class in your program

Add the following declaration to the top of your code:

Then, at some point, you will need to add this inside your program

Once you have created your scanner variable, you can request data and put it into another variable like so:

## Methods of the Scanner class

| **Method** | **Returns** |
| :--- | :--- |
| int nextInt\(\) | Returns the next token as an int. |
| long nextLong\(\) | Returns the next token as a long. |
| float nextFloat\(\) | Returns the next token as a float. |
| double nextDouble\(\) | Returns the next token as a long. |
| String next\(\) | Finds and returns the next complete token from this scanner and returns it as a string; a token is usually ended by whitespace such as a blank or line break. If no token exists, NoSuchElementException is thrown. |
| String nextLine\(\) | Returns the rest of the current line, excluding any line separator at the end. |
| void close\(\) | Closes the scanner object. |

## Your assignment....

Complete the following program. Use the Scanner class to read the following string into variables. Input String: "P Sherman 42 Wallaby Way Sydney" Variables: firstInitial,lastName, houseNumber,streetName,streetType,city

Your output should be handled with this code:

```java
System.out.print(firstInitial + " " + lastName + " " + houseNumber + " ");
System.out.println(streetName + " " + streetType + " " + city);
```

