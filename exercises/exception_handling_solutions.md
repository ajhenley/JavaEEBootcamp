# Exception Handling Solutions

## Exception Assignment

```java
import java.util.Scanner;

class Division {
    public static void main(String[] args) {

        int a, b, result;

        Scanner input = new Scanner(System.in);
        System.out.println("Input two integers");

        a = input.nextInt();
        b = input.nextInt();
        try
        {
            result = a / b;
            System.out.println("Result = " + result);
        }
        catch(ArithmeticException e)
        {
            System.out.println("You cannot divide by zero.");
        }
        finally
        {
            System.out.println("finally block will execute");
        }
    }
}
```

## Finally Clause Assignment

```java
import java.util.Scanner;

class Division {
    public static void main(String[] args) {

        int a, b, result;

        Scanner input = new Scanner(System.in);
        System.out.println("Input two integers");

        a = input.nextInt();
        b = input.nextInt();
        try
        {
            result = a / b;
            System.out.println("Result = " + result);
        }
        catch(ArithmeticException e)
        {
            System.out.println("You cannot divide by zero.");
        }
        finally
        {
            System.out.println("finally block will execute");
        }
    }
}
```

