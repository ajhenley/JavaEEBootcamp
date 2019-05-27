# Comments

## Comments

**Newsflash**: Your memory doesn't work. If you don't believe me then find a program you've written over 6 months or a year ago. Now go through it line by line. Explain to another person the reasons for each line of code in the program.

Try doing that with somebody's else's program.

Now try doing that to a program that contains lots of comments.

What kind of programmer do you want to be?

**Code tells you how. Comments tell you why.**

**Comments are very important in your programs.** They tell you what something does in English. And why.

**Comments can also be used for debugging**. Some programmers will comment out a line of code temporarily while they debug the remaining lines. This enables you to focus on what matters and selectively ignore parts of your program.

**Block comments** Block Comments are shown at the top of the program and they generally contain the name and/or description of the program as well as the programmer's name and the date the program was written.

### Here's how you use comments in Java:

```java
/*
*  Comments Example Program
*  Dave Wolf
*  July 21st, 2015
*/
public class CommentsEverywhere
{
    public static void main( String[] args )
    {
        // This line will be ignored by the compiler
        // but people will (hopefully) read it. 
        // Anything after the // is ignored by Java.
        System.out.println( "This line prints just fine." ); // I can include a comment after the working code..
        // This next line of code has been disabled by a comment:
        // System.out.println("This line won't print.");
        System.out.println( "This line also prints just fine." );
    }
}
```

Programs should be written for people to read. Your code will spend most of its life in maintenance mode. That means a lot of your coworkers - some who may not even be born yet - will have the pleasure of maintaining your program. It's up to you to make sure it's a pleasure.

> The practitioner of literate programming can be regarded as an essayist, whose main concern is with exposition and excellence of style. Such an author, with thesaurus in hand, chooses the names of variables carefully and explains what each variable means. He or she strives for a program that is comprehensible because its concepts have been introduced in an order that is best for human understanding, using a mixture of formal and informal methods that reinforce each other. - Donald Knuth, Literate Programming. 1992.

## Your assignment

* Go through the code below and add comments where you see two slashes. Make sure the code still runs.
* Add a multi-line comment at the top of the program that contains your name, the date and the name of the program.
* If you need information about Random or Scanner then search Oracle's online documentation. There you will find explanations about each.
* Your next assignment is to continue adding comments to your programs as you complete this course

```java
/*
*
*/
import java.util.Random;
import java.util.Scanner;
public class RandomComments
{
    public static void main(String[] args)
    {
        Scanner scan = new Scanner(System.in);

        //
        Random random = new Random();
        long from = 1;
        long to = 100;
        int randomNumber = random.nextInt(to - from + 1) + from;
        //
        int guessedNumber = 0;

        //
        System.out.printf("The number is between %d and %d.\n", from, to);

        //
        do
        {
            System.out.print("Guess what the number is: ");
            guessedNumber = scan.nextInt();
            if (guessedNumber > randomNumber)
                System.out.println("Your guess is too high!");
            else if (guessedNumber < randomNumber)
                System.out.println("Your guess is too low!");
            else
                System.out.println("You got it!");
        } while (guessedNumber != randomNumber);
    }
}
```

