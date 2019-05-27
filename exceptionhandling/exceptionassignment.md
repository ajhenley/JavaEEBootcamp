# Exception Assignment

Create a new application using the code below.

Add Exception Handling to the following code to handle if the user tries to enter zero as the second integer.

```java
import java.util.Scanner;

class Division {
  public static void main(String[] args) {

  int a, b, result;

  Scanner input = new Scanner(System.in);
  System.out.println("Input two integers");

  a = input.nextInt();
  b = input.nextInt();

  result = a / b;

  System.out.println("Result = " + result);
  }
}
```

