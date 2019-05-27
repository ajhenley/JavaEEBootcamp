# Variables

Programs would be pretty boring if all they did was print things on the screen. We would like our programs to be interactive. Variables enable our program to save and retrieve data while the program is runs.

* A variable stores a value that can change as a program executes.
* Before you can use a variable, you must declare its data type and initialize it by assigning a value to it.
* To declare and initialize more than one variable for a single data type in a single statement, use commas to separate the assignments.
* To identify float values, you must type an f or F after the number. To identify long values, you must type an l or L after the number.

**Variables**: If you paid attention in Algebra class you may recall the concept of variable. An equation like `2x + 13 = 25` allows us to find the value of x. What is x? It's a variable that holds a value. Programming languages have variables, too. The concept is the same:

> A variable is a name that refers to a memory location that holds a value.

## Variables in Java have four major differences from math variables:

* Variable names can \(and should\) be more than one letter long
* Variables can store numbers, text or any Java data type
* You set the type of data the variable will hold when declaring it
* The value of a variable can \(and often will\) change. The data type will not change

## The Eight Primitive Data Types

Use a data type that is appropriate for the data you're storing. Write primitive data type names using lower-case.

| Type | Bytes | Use |
| :--- | :--- | :--- |
| byte | 1 | Short integers from -128 to 127. |
| short | 2 | Short integers from -32,768 to 32,767. |
| int | 4 | Integers from -2,147,483,648 to 2,147,483,647 |
| long | 8 | Long integers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |
| float | 4 | Single-precision, floating-point numbers from -1.7E308 to 1.7E308 with up to 16 significant digits. |
| char | 2 | A single Unicode character that's stored in two bytes. |
| boolean | 1 | A true or false value. |

## How to declare and initialize a variable in two statements\|

```java
int counter;
counter = 1;
```

## How to declare and initialize a variable in one statement

```java
int counter = 1;
```

## Examples:

```java
double price = 14.95;
float interestRate = 8.125F;
long numberOfBytes = 2000L;
int population = 1734323;
int popluation = 1_734_423;
double distance = 3.65e+9;
char letter = 'A';
char letter = 65;
boolen valid = false;
int x = 0, y = 0;
```

```java
/* VariousVaribles - a program to teach us about variables
*/
public class VariousVariables
{
    public static void main( String[] args )
    {
        //declare variables here before we use them
        int x, y, answer; //all three variables will be declared as integers
        double temperature;
        float  Temperature; //a float uses less memory than a double
        String firstName, lastName;
        String question = "unknown"; //question is initialized

        //assign values to the variables here
        x = 99;
        y = 2147483647; //you could also use the constant Integer.MAX_VALUE
        answer = 42;
        firstName = "James";
        lastName = "Gosling";
        temperature = 98.6;
        Temperature = 32.0f;

        //Use the variables here
        System.out.println( "The variable x contains a value of " + x );
        System.out.print( "The value " + y + " is the largest value ");
        System.out.println( "you can store in an integer." );
        System.out.println("The anwser to the question is: " + answer );
        System.out.println("And the question has long since been " + question);
        System.out.println("If you're not sick your temperature is " 
                                                                + temperature);
        System.out.println("If you're an ice cube your temperature is " 
                                                                + Temperature);
        System.out.println("The variable Temperature is not "
                                                 + "the same as  temperature");
        System.out.println("The founder of Java is " + firstName + lastName );
    }
}
```

## What You Should See

```text
The variable x contains a value of 99
The value 2147483647 is the largest value you can store in an integer.
The anwser to the question is: 42
And the question has long since been unknown
If you're not sick your temperature is 98.6
If you're an ice cube your temperature is 32.0
The variable Temperature is not the same as  temperature
The founder of Java is JamesGosling
```

At the top of the program we declare the variables. It's common practice to declare variables at the top of your method or class. Variables declared within a method are visible only within that method.

You want to choose the appropriate data type for your variable. Names are stored as `String` variables. Numbers without decimal points are stored as `int` variables.

A float uses less memory than a double. Floats should not be used for precise values, such as currency. The `java.math.BigDecimal` class is intended for currency values since it is more accurate. We'll look at that later.

## What you should do

1. Copy the above program to Eclipse and be able to generate the same output shown above. 
2. Modify the variables to print your name and age. 
3. Put a space between your first and last names.
4. Add a variable for the last movie you saw. 
5. Add a variable for your GPA. Display that. If you don't like your GPA make one up.

