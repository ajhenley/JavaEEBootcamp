# Basic Java Answers

## Basic Java Solutions

### Your first java program

```java
public class HelloWorld
 {
    public static void main( String[] args )
    {
        System.out.println( "Hello, World!" );
        System.out.println("Today is July 19, 2015. I am alive!");
        System.out.println("My name is Alton.");
    }
 }
```

### More Printing

```java
public class PrintReceipt
{
  public static void main( String[] args )
  {
      System.out.println( "+--------------------------------------+");
      System.out.println( "|      Java Bank ATM Receipt           |");
      System.out.println( "|      Wednesday, December 2, 2015     |");
      System.out.println( "|      ATM Location # 123              |");
      System.out.println( "|                                      |");
      System.out.println( "|                                      |");
      System.out.println( "|      Account Number:      1234567    |");
      System.out.println( "|      Customer:     John Q. Public    |");
      System.out.println( "|      Transaction Type:    Deposit    |");
      System.out.println( "|      Transaction Amount:  $500.00    |");
      System.out.println( "|      Account Balance:   $1,500.00    |");
      System.out.println( "|                                      |");
      System.out.println( "|      Thank you for banking with us   |");
      System.out.println( "|            Have a coffee day         |");
      System.out.println( "|                                      |");
      System.out.println( "+--------------------------------------+");
  }
}
```

### A program for yourself

```java
public class MyProgram
 {
    public static void main( String[] args )
    {
        // My name is Alton
        // I am 47 years old
    }
 }
```

### Debug this program

```java
public class DebugProg {
    public static void main(String[] args) {
        double x, y;

        x = 3.1415;
        y = 3.64;

        System.out.println("pi is approximately " + x);
        System.out.println("My GPA was " + y);
    }
}
```

### Math two

```java
public class MathTwoProg {
    public static void main(String[] args) {
        int myNumber;
        double myOtherNumber;

        myNumber = 2;
        myOtherNumber = 1.7938;

        System.out.println("myNumber is " + myNumber);
        System.out.println("myOtherNumber is " + myOtherNumber);
    }
}
```

### Change Program

```java
public class ChangeProgram {
    public static void main(String[] args) {
        int x;
        double y, z;

        x = 5;
        y = 8.75;

        z = x * y;

        System.out.println("The product is " + z);
    }
}
```

### Getting and Storing User Input

```java
import java.util.Scanner;

public class GettingInput {
    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);

        String firstInitial = keyboard.next();
        String lastName = keyboard.next();
        int houseNumber = keyboard.nextInt();
        String streetName = keyboard.next();
        String streetType = keyboard.next();
        String city = keyboard.next();

        System.out.print(firstInitial + " " + lastName + " " + houseNumber + " ");
        System.out.println(streetName + " " + streetType + " " + city);
    }
}
```

### String Completion Assignment

```java
import java.util.Scanner;

public class PetQuestions {
    public static void main(String[] args) {
        String name;
        String breed;
        int age;

        Scanner keyboard = new Scanner(System.in);

        System.out.print( "Greetings. What is your pet's name? " );
        name = keyboard.next();

        System.out.print( "What kind of animal is " + name + "? " );
        breed =keyboard.next();

        System.out.print( "How old is " + name + "? ");
        age = keyboard.nextInt();

        System.out.println( name + " is your " + breed + " and it is " + age );
    }
}
```

### String Assignment

```java
public class StringAssignment {
    public static void main(String[] args) {
        String name = "Alton";
        System.out.print(name);
    }
}
```

### Special Characters Assignment

```java
public class SpecialCharacters {
    public static void main(String[] args) {
        String message1, message2;

        message1 ="message1 = \\/\\/\\/\\/\\/\\r\\t\\b ";
        message2 = "\nmessage2 = \";";

        System.out.println(message1 + message2);
    }
}
```

Need it explained? Then watch the video walkthrough...  
 [Video Walkthrough - http://links.learningbycoding.com/specialchars](https://ajhenley.wistia.com/medias/hgvfnibluf)

### Output Assignment

```java
import java.util.Scanner;

public class SomethingAboutYou
{
    public static void main( String[] args )
    {
        Scanner sc = new Scanner(System.in);

        String firstName;
        int age;
        String height;
        double gpa;

        System.out.print( "What is your first name? " );
        firstName = sc.next();

        System.out.print( "How old are you? " );
        age = sc.nextInt();

        System.out.print( "How tall are you? " );
        height = sc.next();

        System.out.print( "What is your GPA? " );
        gpa = sc.nextDouble();

        System.out.println("You are " + firstName);
        System.out.println("You are " + age + " years old.");
        System.out.println("Your height is: " + height);
        System.out.print("Your awesome gpa is: " + gpa);

        sc.close();
     }
}
```

### Input Output Debugging Assignment

```java
import java.util.Scanner;

public class AskingQuestions
{
    public static void main( String[] args )
    {
        Scanner keyboard = new Scanner(System.in);

        int num1, num2, num3;

        System.out.print( "First integer? " );
        num1 = keyboard.nextInt();

        System.out.print( "Second integer? " );
        num2 = keyboard.nextInt();

        System.out.print( "Third integer? " );
        num3 = keyboard.nextInt();

        System.out.println("The total is : " + (num1 + num2 + num3));
    }
}
```

### Input Output Change Assignment

```java
import java.util.Scanner;

public class AskingQuestions
{
    public static void main( String[] args )
        Scanner keyboard = new Scanner(System.in);

        int num1, num2, num3;

        System.out.print( "First temperature? " );
        num1 = keyboard.nextInt();

        System.out.print( "Second temperature? " );
        num2 = keyboard.nextInt();

        System.out.println("The max value is : " + (num1 + num2) / 2);
    }
}
```

## Mowing Time Programming Activity

```java
import java.util.Scanner;

public class MowingTime
{
  public static void main( String[] args )
  {
    Scanner keyboard = new Scanner(System.in);
    double length, width, lawnArea;

    System.out.print( "Lawn length? " );
    length = keyboard.nextDouble();

    System.out.print( "Lawn width? " );
    width = keyboard.nextDouble();

    lawnArea = length * width;

    System.out.println("The are of the lawn is " + lawnArea + 
      " sq yard, and Bob can mow it in "+ (lawnArea / 40 * 2) + 
      " minutes.");

    keyboard.close();
  }
}
```

### More Mowing Time

```java
import java.text.NumberFormat;
import java.util.Scanner;

public class MowingAssignment
{
    public static void main( String[] args )
    {
        Scanner keyboard = new Scanner(System.in);
        NumberFormat currency = NumberFormat.getCurrencyInstance();

        //keep the rates as constants to make updates and changes easier
        final int lawnTimeRate= 2;
        final int lawnCostRate = 12 ;

        double yardLength, yardWidth, houseLength, houseWidth, lawnArea, lawnTimeHrs;

        System.out.print( "What is the yard length? " );
        yardLength = keyboard.nextDouble();

        System.out.print( "What is the yard width?" );
        yardWidth = keyboard.nextDouble();

        System.out.print( "What is the house length? " );
        houseLength = keyboard.nextDouble();

        System.out.print( "What is the yard width?" );
        houseWidth = keyboard.nextDouble();

        lawnArea = (yardLength * yardWidth) - (houseLength * houseWidth); 

        //convert time from minutes to hours 
        lawnTimeHrs= (lawnArea / 40 * lawnTimeRate) / 60;

        System.out.println("The area of the lawn that needs to be mowed is " 
          + lawnArea + " sq yar. It will take "+ lawnTimeHrs + 
          " hours to finish the mowing and will cost " + 
          currency.format((float)(lawnTimeHrs * lawnCostRate)) + ".");

        System.out.println("If Bob charges $45 per lawn, " + 
          "then the profit will be: " + 
          currency.format((float)(45 - lawnTimeHrs * 45)));

        keyboard.close();
    }
}
```

### What If Change Activity

```java
import java.util.Scanner;

public class StudentRecordReader {
    public static void main(String[] args) {
        String fname, lname, status;
        double gpa;
        int hours;

        Scanner keyboard = new Scanner(System.in);

        System.out.print( "Student's First Name? " );
        fname = keyboard.next();

        System.out.print( "Student's Last Name? " );
        lname = keyboard.next();

        System.out.print( "Student's GPA? " );
        gpa = keyboard.nextDouble();

        System.out.print( "Student's Current Course Load? " );
        hours = keyboard.nextInt();

        if (hours >= 12)
        {
            System.out.println();
            System.out.println("Student Name :" + fname + " " + lname);
            System.out.println("Student GPA :" + gpa);
            if (gpa >= 3)
            {
                System.out.println("This student is in good standing.");
            } else if (gpa >= 2)
            {
                System.out.println("This student needs to study more.");
            } else if (gpa >= 1)
            {
                System.out.println("This student is on academic probation.");
            } else
            {
                System.out.println("This student has been expelled.");
            }
        }
    }
}
```

### What if debugging activity

```java
import java.util.Scanner;

public class StudentRecordReader {

    public static void main(String[] args) {
        String fname, lname;
        double gpa;

        Scanner keyboard = new Scanner(System.in);

        System.out.print( "Student's First Name? " );
        fname = keyboard.next();

        System.out.print( "Student's Last Name? " );
        lname = keyboard.next();

        System.out.print( "Student's GPA? " );
        gpa = keyboard.nextDouble();

        System.out.println();
        System.out.println("Student Name :" + fname + " " + lname);
        System.out.println("Student GPA :" + gpa);
        if (gpa >= 3)
        {
            System.out.println("This student is in good standing.");
        } else if (gpa >= 1)
        {
            System.out.println("This student is on academic probation.");
        } else
        {
            System.out.println("This student has been expelled.");
        }
    }
}
```

### Comparing strings activity

```java
import java.util.Scanner;

public class MyWeatherMan {

    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        System.out.println("How is the weather?");
        String answer = sc.nextLine();

        if (answer.equals("rain"))
            System.out.println("Take your umbrella!");
        else if (answer.equals("windy"))
            System.out.println("Wear your jacket!");
        else if (answer.equals("snow") )
            System.out.println("Wear a coat and take a shovel!");
        else if (answer.equals("stormy")
            System.out.println("Stay Inside!");
        else
            System.out.println("Enjoy your day!");
     }
}
```

### What if completion activity

```java
import java.util.Scanner;

public class PairProcess {
    public static void main(String[] args) {
        int num1, num2;

        Scanner keyboard = new Scanner(System.in);

        System.out.print( "First Number? :" );
        num1 = keyboard.nextInt();

        System.out.print( "Last Number?  :" );
        num2 = keyboard.nextInt();

        System.out.println("sum     : " + (num1 + num2));
        System.out.println("product : " + (num1 * num2));
        System.out.println("average : " + (num1 + num2)/2 );
    }
}
```

#### bonus question

```java
import java.util.Scanner;

public class PairProject {
    public static void main(String[] args) {
        int num1, num2;

        Scanner keyboard = new Scanner(System.in);

        System.out.print( "First Number? :" );
        num1 = keyboard.nextInt();

        System.out.print( "Last Number?  :" );
        num2 = keyboard.nextInt();

        if ((num1+num2) < 1000)
        {
            System.out.println("sum     : " + (num1 + num2) + "~");
        } else
        {
            System.out.println("sum     : " + (num1 + num2) );
        }
        System.out.println("product : " + (num1 * num2));
        System.out.println("average : " + (num1 + num2)/2 );
    }
}
```

### What If activity

```java
import java.util.Scanner;

public class SalesRecord {
    public static void main(String[] args) {
        String custnum, name, taxcode;
        double salesamt;

        Scanner keyboard = new Scanner(System.in);

        System.out.print("Customer Number : ");
        custnum = keyboard.next();

        System.out.print("Name : ");
        name = keyboard.next();

        System.out.print("Sales amount : $");
        salesamt = keyboard.nextDouble();

        System.out.print("Tax Code : ");
        taxcode = keyboard.next();

        if (taxcode.equals("NRM"))
            System.out.println("Total (with tax) : $" + (salesamt * 1.06));
        else if (taxcode.equals("NPF"))
            System.out.println("Total (with tax) : $" + (salesamt * 1));
        else if (taxcode.equals("BIZ"))
            System.out.println("Total (with tax) : $" + (salesamt * 1.04555));
    }
}
```

### Randomness Debugging Activity

```java
import java.util.Random;

public class RandomGenerator{
    public static void main(String[] args)
    {
        output("Generate 10 random integers between 1 and 6");

        Random rnd = new Random();

        for (int i = 1; i <= 10; ++i)
        {
          int randomInt = 1 + rnd.nextInt(6);
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

### Randomness Change Activity

```java
import java.util.Random;

public class RandomGenerator{
    public static void main(String[] args)
    {
        System.out.println("Generate 10 random integers between 5 and 95");

        Random rnd = new Random();

        for (int i = 1; i <= 10; ++i)
        {
          int randomInt = 5 + rnd.nextInt(91);
          System.out.println("Generated number: " + randomInt);
        }

        System.out.println("Done.");
    }
}
```

### Randomness completion activity

```java
import java.util.Random;

public class DiceRoller
 {
    public static void main( String[] args )
    {
        int dienumber;
        Random rnd = new Random();

        dienumber = 1 +rnd.nextInt(6);

        System.out.println("Your die roll was : " + dienumber);
    }
 }
```

### Repeating yourself with the while loop

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
            if (guess==5)
            {
                break;
            }
        }

        System.out.println("You are correct. You win a prize!");
        keyboard.close();
    }
}
```

### Guessing Game

```java
import java.util.Random;
import java.util.Scanner;

public class GuessingGame {
    public static void main(String[] args)
    {
        Random rnd = new Random();
        Scanner keyboard =  new Scanner(System.in);
        int guess;
        boolean notDone = true;
        int myNumber = rnd.nextInt(10) + 1;

        System.out.println(
          "I have chosen a number between 1 and 10. Try to guess it.");

        while(notDone)
        {
            System.out.println("Your guess: ");
            guess = keyboard.nextInt();

            if (guess == myNumber)
            {
                System.out.println("That's right! You're a good guesser.");
                notDone = false;
            } else {
                System.out.println("That is incorrect. Guess again.");
            }
        }
    }
}
```

### For Loop Activity

```java
public class BottlesOfBeer {
    public static void main(String[] args) {
        for (int i = 100; i >= 1; i--)
        {
            System.out.printf("%d bottles of beer in the wall.", i);
            System.out.println();
            System.out.printf("%d bottles of beer.", i);
            System.out.println();
            System.out.println("If one of the bottles should happen to fall,");
            System.out.printf("%d bottles of beer in the wall", i - 1);
            System.out.println();
            System.out.println();
        }
    }
}
```

### Nested For Loop Activity

```java
public class NestedForLoops {
    public static void main(String[] args) {
        for (int i = 1; i<10; i++)
        {
            for (int j = 1; j <= i; j++)
            {
                System.out.print(i);
            }
            System.out.println();
        }
    }
}
```

### Loop Debugging Activity

```java
import java.util.Scanner;

public class StopSayingThat {
    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);

        String userInput = "";
        userInput = keyboard.next();

        while ( userInput != "" )
        {
            System.out.println(userInput);            
        }
    }
}
```

### Loop Completion Activity

```java
import java.util.Scanner;

public class GetIntegers {
    public void main (String[] args)
    {
        Scanner keyboard = new Scanner(System.in);

        int num, total = 0;

        for (int i = 1; i <= 10; i++)
        {
          num = keyboard.nextInt();
          total += num;
        }
        System.out.println("The total of all 10 numbers is " + total);
    }
}
```

### A variation of the dice game Pig

```java
import java.util.Random;
import java.util.Scanner;

public class Pig {

    public static void main(String[] args) {
        int die1, die2;
        int score = 0;
        Scanner keyboard = new Scanner(System.in);

        String again = "y";
        Random rnd = new Random();

        while (again.equals("y"))
        {
            die1 = 1 + rnd.nextInt(6);
            die2 = 1 + rnd.nextInt(6);

            if (die1 + die2 == 2)
            {
                score = score + 25;
            } else if (die1 > 1 && die2 > 1){
                score = score + die1 + die2;
            } 

            System.out.printf("You roll: %d and %d. Your score is %d.\n", die1, die2, score);

            if (score < 100)
            {
                System.out.println("Press Y to roll again.");
                again = keyboard.next();
            } 
                else
            {
                System.out.println("Game Over. You Win!");
                again="n";
            }
        }
    }
}
```

### Zork

```java
import java.util.Scanner;

public class Zork {
    public final static int WINDOW = 0;
    public final static int FOYER = 1;
    public final static int FRONT = 2;
    public final static int LIBRARY = 3;
    public final static int KITCHEN = 4;
    public final static int DINING = 5;
    public final static int VAULT = 6;
    public final static int PARLOR = 7;

    public static void main(String[] args) {

        Scanner keyboard = new Scanner(System.in);
        int input, room = FOYER;
        String quit = "anything";


        do {

            // foyer
            if (room == FOYER) {
                System.out.println("You are standing in the foyer of an old house.");
                System.out.println("You see a dead scorpion.");
                System.out.print("You can (1) exit to the north, (2) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = FRONT;
                else if (input == 2)
                    quit = "run";

                // front room
            } else if (room == FRONT) {
                System.out.println("You are standing in the front room.");
                System.out.println("You see a piano.");
                System.out.println("You can (1) exit to the south, (2) exit to the east, (3) exit to the west, (4) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = FOYER;
                else if (input == 2)
                    room = LIBRARY;
                else if (input == 3)
                    room = KITCHEN;
                else if (input == 4)
                    quit = "run";

                // library
            } else if (room == LIBRARY) {
                System.out.println("You are standing in the library.");
                System.out.println("You see a spiders.");
                System.out.println("You can (1) exit to the west, (2) exit to the north, (3) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = 2;
                else if (input == 2)
                    room = 5;
                else if (input == 3)
                    quit = "run";

                // kitchen
            } else if (room == KITCHEN) {
                System.out.println("You are standing in the kitchen.");
                System.out.println("You see a bats.");
                System.out
                        .println("You can (1) exit to the east, (2) exit to the north, (3) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = 2;
                else if (input == 2)
                    room = 7;
                else if (input == 3)
                    quit = "run";

                // dining room
            } else if (room == DINING) {
                System.out.println("You are standing in the dining room.");
                System.out.println("You see a dust and empty box.");
                System.out.println("You can (1) exit to the south, (2) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = 3;
                else if (input == 2)
                    quit = "run";

                // vault
            } else if (room == VAULT) {
                System.out.println("You are standing in the vault.");
                System.out.println("You see a three walking skeletons.");
                System.out.println("You can (1) exit to the east, (2) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = 7;
                else if (input == 2)
                    quit = "run";

                // parlor
            } else if (room == PARLOR) {
                System.out.println("You are standing in the parlor.");
                System.out.println("You see a treasure chest.");
                System.out
                        .println("You can (1) exit to the west, (2) exit to the south, (3) run. ");

                input = keyboard.nextInt();
                if (input == 1)
                    room = 6;
                else if (input == 2)
                    room = 4;
                else if (input == 3)
                    quit = "run";
            }
        } while (!quit.equals("run"));
        System.out.println("You have exited!");
        keyboard.close();
    }
}
```

### Switch Statement Activity

```java
import java.util.Scanner;

public class HoleInTen {
    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);
        String prodCode;

        System.out.println("Product Code? ");
        prodCode = keyboard.next();

        switch (prodCode) {
        case "BALL": System.out.println("Golf Balls (1 dozen) @ 38.00");
            break;
        case "DRV01": System.out.println("Big Bertha Driver @ $449.95");
            break;
        case "DRV02": System.out.println("Vaporizer Driver @ $375.00");
            break;
        case "DRV03": System.out.println("Fly-Z Driver @ $179.00");
            break;
        case "SET01": System.out.println("Project Manager Golf Club Set @ $179.00");
            break;
        case "SET02": System.out.println("Project Manager Golf Club Set @ $225.00");
            break;
        case "SET03": System.out.println("Executive Golf Club Set @ $299.95");
            break;
        case "SET04": System.out.println("CEO Golf Club Set @ $374.95");
            break;
        case "SET05": System.out.println("Chairman of the Board Club Set @ $495.00");
            break;
        default: System.out.println("Invalid Product");
        }
    }
}
```

### An array to remember

```java
import java.util.Scanner;

public class RememberArray {
    static Scanner sc = new Scanner(System.in);
    static int maxItems = 100;
    static String[] memory = new String[maxItems];
    static int currentItems = 0;

    public static void main(String[] args)
    {
        getUserInput(); //An Array to Remember
        sortAndDisplay(); //Bonus Basic Java Assignment

    }

    private static void getUserInput()
    {
        String input = "";
        System.out.println("Type \'history\' to display remembered phrases starting from most recent.");
        System.out.println("Type \'quit\' to stop input.");
        while(!input.equalsIgnoreCase("quit") && currentItems < maxItems)
        {
            System.out.print("Input word or phrase: ");
            input = sc.nextLine();
            if(input.equalsIgnoreCase("history"))
            {
                rememberHistory();
            }
            else if(input.equalsIgnoreCase("quit"))
            {
                System.out.println("You have chosen to end entry.");
            }
            else
            {
                commitToMemory(input);
            }
        }
    }

    private static void commitToMemory(String thing)
    {
        memory[currentItems] = thing;
        currentItems++;
    }

    private static void rememberHistory()
    {
        for(int i = currentItems - 1; i >= 0; i--)
        {
            System.out.println(memory[i]);
        }
    }

    private static void sortAndDisplay()
    {
        String temp = "";
        System.out.println("Alphabetically sorted: ");
        //Sort
        for(int i = 0; i < currentItems - 1; i++)
        {
            for(int j = 1; j < currentItems - i; j++)
            {
                if(memory[j - 1].compareToIgnoreCase(memory[j]) > 0)
                {
                    temp = memory[j - 1];
                    memory[j - 1] = memory[j];
                    memory[j] = temp;
                }
            }
        }
        //Display
        for(int k = 0; k < currentItems; k++)
        {
            System.out.println(memory[k]);
        }
    }
}
```

### Working with files

```java
import java.util.Scanner;
import java.io.PrintWriter;
import java.io.IOException;
import java.io.File;
import java.io.BufferedReader;
import java.io.FileReader;

public class ReadWriteTemperatures {

    public static void main(String[] args)
    {
        Scanner keyboard = new Scanner(System.in);
        String result;

        try {

            File file = new File("temperatures");        
            file.createNewFile();

            PrintWriter pw = new PrintWriter(file);

            for (int i=1; i <= 15; i++)
            {
                System.out.print("Enter a temperature:");
                result = keyboard.nextLine();
                pw.println(result);
            }

            pw.flush();
            pw.close();

            //read our file
            FileReader fr = new FileReader(file);
            BufferedReader br = new BufferedReader(fr);
            String line;
            while ( (line = br.readLine())!= null)
            {
                System.out.println(line);
            }
            br.close();


        } catch (IOException e) {
            System.out.println("Oops! An error occurred.");
        } finally {
            keyboard.close();
        }
    }
}
```

### Finding words with the do-while loop

```java
import java.io.BufferedReader;
import java.io.File;
import java.io.FileReader;
import java.util.Scanner;

public class WordFinder {

    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);
        String word = "";
        boolean found = false;
        int i = 0;

        do {
            System.out.println("Please enter a word to lookup: ");
            word = keyboard.next();
        } while (word.length() == 0);

        try{
            File file = new File("/usr/share/dict/words");

            FileReader fr = new FileReader(file);
            BufferedReader br = new BufferedReader(fr);
            String line;
            while( (line = br.readLine()) != null)
            {
                i++;
                if (line.equals(word))
                {
                    System.out.println(word + " found at position #" + i );
                    found = true;
                    break;
                }
            }

            if (!found) 
            {
              System.out.println(
              "After checking " + i + " words, your word was not found"); 
            }
            br.close();
        }
        catch(Exception e) {
            System.out.println("Oops! An error occurred.");
        } finally {
            keyboard.close();
        }
    }
}
```

### Gift Advisor

```java
import java.util.Scanner;

public class GiftAdvisor {
    static Scanner sc = new Scanner(System.in);

    public static void main(String[] args)
    {
        determineGift();
    }

    private static void determineGift()
    {
        String gender = getGender();
        String priceRange = getPriceRange();
        String ageRange = getAgeRange();
        String gift = recommendGift(gender, priceRange, ageRange);
        if(gift.equalsIgnoreCase("gift certificate"))
        {
            System.out.println("No ideas. Give " + gift);
        }
        else
        {
            System.out.println("Recommended gift(s): " + gift);
        }
    }

    private static String getGender()
    {
        System.out.print("Input recipient's gender: ");
        String gender = sc.next();
        return gender;
    }

    private static String getPriceRange()
    {
        System.out.print("Input giver\'s price range: ");
        String priceRange = sc.next();
        return priceRange;
    }

    private static String getAgeRange()
    {
        System.out.print("Input recipient's age range: ");
        String ageRange = sc.next();
        return ageRange;
    }

    private static String recommendGift(String gender, String priceRange, String ageRange)
    {
        String recommendedGift = "";
        if(gender.equalsIgnoreCase("male"))
        {
            if(priceRange.equalsIgnoreCase("low"))
            {
                if(ageRange.equalsIgnoreCase("adult"))
                {
                    recommendedGift = "Books";
                }
                else if(ageRange.equalsIgnoreCase("teen"))
                {
                    recommendedGift = "Shoes";
                }
                else if(ageRange.equalsIgnoreCase("child"))
                {
                    recommendedGift = "SD Gunpla";
                }
                else
                {
                    recommendedGift = "gift certificate";
                }
            }
            else if(priceRange.equalsIgnoreCase("medium"))
            {
                if(ageRange.equalsIgnoreCase("adult"))
                {
                    recommendedGift = "Guitar";
                }
                else if(ageRange.equalsIgnoreCase("teen"))
                {
                    recommendedGift = "Playstation";
                }
                else if(ageRange.equalsIgnoreCase("child"))
                {
                    recommendedGift = "HG Gunpla";
                }
                else
                {
                    recommendedGift = "gift certificate";
                }
            }
            else if(priceRange.equalsIgnoreCase("high"))
            {
                if(ageRange.equalsIgnoreCase("adult"))
                {
                    recommendedGift = "Smart TV";
                }
                else if(ageRange.equalsIgnoreCase("teen"))
                {
                    recommendedGift = "Apple Watch";
                }
                else if(ageRange.equalsIgnoreCase("child"))
                {
                    recommendedGift = "MG Gunpla";
                }
                else
                {
                    recommendedGift = "gift certificate";
                }
            }
            else
            {
                recommendedGift = "gift certificate";
            }
        }
        else if(gender.equalsIgnoreCase("female"))
        {
            if(priceRange.equalsIgnoreCase("low"))
            {
                if(ageRange.equalsIgnoreCase("adult"))
                {
                    recommendedGift = "Wine";
                }
                else if(ageRange.equalsIgnoreCase("teen"))
                {
                    recommendedGift = "Selfie Stick";
                }
                else if(ageRange.equalsIgnoreCase("child"))
                {
                    recommendedGift = "Teddy Bear";
                }
                else
                {
                    recommendedGift = "gift certificate";
                }
            }
            else if(priceRange.equalsIgnoreCase("medium"))
            {
                if(ageRange.equalsIgnoreCase("adult"))
                {
                    recommendedGift = "Perfume";
                }
                else if(ageRange.equalsIgnoreCase("teen"))
                {
                    recommendedGift = "Sweater";
                }
                else if(ageRange.equalsIgnoreCase("child"))
                {
                    recommendedGift = "53\" Hugfun Bear";
                }
                else
                {
                    recommendedGift = "gift certificate";
                }
            }
            else if(priceRange.equalsIgnoreCase("high"))
            {
                if(ageRange.equalsIgnoreCase("adult"))
                {
                    recommendedGift = "Weekend Getaway";
                }
                else if(ageRange.equalsIgnoreCase("teen"))
                {
                    recommendedGift = "Jewelry";
                }
                else if(ageRange.equalsIgnoreCase("child"))
                {
                    recommendedGift = "93\" Hugfun Bear";
                }
                else
                {
                    recommendedGift = "gift certificate";
                }
            }
            else
            {
                recommendedGift = "gift certificate";
            }
        }
        else
        {
            recommendedGift = "gift certificate";
        }
        return recommendedGift;
    }
}
```

