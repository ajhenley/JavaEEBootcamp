# What does this code do? Part 1

When programmers develop a program or some code they spend some amount of time creating it. The code then goes into production and may be run for weeks, months, years, or decades. The IRS is still using programs developed in the early 1970's. Those programs have changed since their first inception. Imagine the number of new tax laws that have to be added to the IRS program's code each year. Estimates vary, but over 80% of your code's lifetime will be spent in maintenance. That means you should give your variables meaningful names. It also means you should use comments generously. This will make it easier for the next person to maintain your program.

Here's an example of a well-written program. You should find it easy to follow the intent of the programmer.

```java
/*
 * PalindromeTester.java
 * 
 * Tests a string as entered by the user 
 * to see whether or not it is a palindrome or not.
 * A palindrome would be the same string forwards 
 * as it is backwards.
 * Examples: Anna, civic and of, course:
 * A man a plan a canal Panama.
 */
import java.util.*;

public class PalindromeTester {
    public static void main(String[] args) {
        // The palindrome will be entered by the user at the keyboard
        Scanner in = new Scanner(System.in);

        System.out.println("Palindrome Checker");
        System.out.print("What phrase would you like to check? ");
        String original = in.nextLine();

        // Convert to lower case to simplify comparing strings
        String phrase = original.toLowerCase(); 

        String backwards = ""; 

        // loop through the string backwards, starting with the last character
        for (int i = phrase.length() - 1; i >= 0; i--) {

            // Extract each letter as the next character 
            // and build the backwards string
            String letter = phrase.substring(i, i + 1);
            backwards += letter;
        }        

        // A palindrome is a word or phrase that is the same forward or 
        // backward. This is where we check that.
        if (phrase.equals(backwards)) {
            System.out.println(original + " is a palindrome!");
        } else {
            System.out.println(original + " is not a palindrome!");            
        }

    }
}
```

