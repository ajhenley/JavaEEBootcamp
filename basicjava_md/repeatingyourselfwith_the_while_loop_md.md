# Repeating yourself with the while loop

You are going to learn how to make sections of your code repeat. This will give you the ability to reuse your code so you don't have to write the same code multiple times.

The while loop is good when you don't know how many times a block of code should repeat. The while loop will continue as long as some condition it true. It looks like this:

```java
while (expression) {
 // do you thing as long as the expression is true
}
```

The while loop will never run if the expression isn't true. There are lots of times when the while loop may not even run.

```java
bool run = false;
while (run){
    //this code would never run
}
```

```java
import java.util.Scanner;

public class KeepGuessing {
    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);
        int secretNumber, guess = 0;//guess is initialized to 0

        secretNumber = 123;

        System.out.println("I'm thinking of a number between 1 and 1000");
        System.out.print("Enter the number:");
        guess = keyboard.nextInt();

        while ( guess != secretNumber )
        {
            System.out.println("\nYou are wrong. Try again.");
            System.out.println("Enter the number: ");
            guess = keyboard.nextInt();
        }

        System.out.println("You are correct. You win a prize!");
        keyboard.close();
    }
}
```

## Your assignment

The while loop will continue until the test condition is true. You can also break out of a while loop by using the keyword `break`. Modify the above program to also exit the while loop if the person guesses "5".

