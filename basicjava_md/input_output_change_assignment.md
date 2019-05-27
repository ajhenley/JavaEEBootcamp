# Input output change assignment

This application takes 2 integer values and finds the largest one. Change the application so that it finds the average of two double values.

```java
import java.util.Scanner;

public class AskingQuestions
{
    public static void main( String[] args )
    {
        Scanner keyboard = new Scanner(System.in);

        int num1, num2, num3;

        System.out.print( "First temperature? " );
        num1 = keyboard.nextInt();

        System.out.print( "Second temperature? " );
        num2 = keyboard.nextInt();

        System.out.println("The max value is : " + Math.max(num1, num2));
    }
}
```

