# Randomness

You know what's cool? Having the computer randomly choose a number. This is the basis of pretty much every computer game ever. To pick a random number, you first need to import `java.util.Random;` Then, you must create a random-number generator object, like so:

```java
Random rnd = new Random();
```

Once that's finished, you can have the computer pick a random integer like this:

```java
int x = 1 + rnd.nextInt(100);
```

That picks a random number from 1 to 100 \(inclusive\) and store it into the variable x. Let's look at some code!

```java
import java.util.Random;

public class RandomGenerator{
    public static void main(String[] args)
    {
        output("Generate 10 random integers between 0 and 99");

        Random rnd = new Random();

        for (int i = 1; i <= 10; ++i)
        {
          int randomInt = 1 + rnd.nextInt(100);
          output("Generated number: " + randomInt);
        }

        output("Done.");
    }

  private static void output(String aMessage)
  {
    System.out.println(aMessage);
  }
}
```

1. Delete the 1 + from the line that reads `int randomInt = 1 + rnd.nextInt(100);`.Run the program to see what this does to the range of the random numbers.
2. Change the 1 + from the line that read `int randomInt = 1 + rnd.nextInt(100);` to `5 +`. What happens?
3. Change the line where you create the random number generator so that it looks like this: Random r = new Random\(23456\); This number is called a seed. Run the program a few times. What happens?
4. Change to random seed to something else. What happens?
5. If you cast a number to a \(char\) then the character representation of that number will be printed. Create a password generator that casts 8 random numbers between 40 and 126 to characters. 

