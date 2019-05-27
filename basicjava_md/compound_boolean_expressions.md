# Compound boolean expressions

Sometimes we want to use logic more complicated than just “less than” or “equal to”.

For example, project managers are constantly asking programmers to write new software. And they want it done fast, cheap and perfect. However, any good programmer will tell you that the rule is: **We can make it fast, cheap or good. Pick two**.

```java
import java.util.Scanner;

public class ProjectManagerDecisionMaker {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        boolean bFast = false;
        boolean bCheap = false;
        boolean bGood = false;

        System.out.print("Do you want it fast? (y/n) ");
        String fast  = scan.nextLine();
        if (fast.equals("y")){
            bFast = true;
        }

        System.out.print("Do you want it cheap? (y/n) ");
        String cheap = scan.nextLine();
        if (cheap.equals("y")){
            bCheap = true;
        }

        System.out.print("Do you want it to be good? (y/n) ");
        String good = scan.nextLine();
        if (good.equals("y")){
            bGood = true;
        }

        if (bFast != true && bCheap == true && bGood == true)
            System.out.println("OK, we'll make it cheap and good. But it will take a while.");
        else if (bFast == true && bCheap !=true && bGood == true)
            System.out.println("OK, we'll make it good and have it to you quickly. But it will cost you!");
        else if (bFast == true && bCheap == true && bGood != true)
            System.out.println("Ok, it will be done right away and it won't cost you much but it won't be very good!" );
        else
            System.out.println("Sorry, you can only have two.");

    }

}
```

For complicated Boolean expressions you can use parentheses to group things, and you use the symbols && to mean “AND” and the symbols \|\| to mean “OR”.

## Truth table for AND:

| Inputs | Output\(s\) |  |
| :--- | :--- | :--- |
| A | B | A && B |
| true | true | true |
| true | false | false |
| false | true | false |
| false | false | false |

## Truth table for OR:

| Inputs | Output\(s\) |  |
| :--- | :--- | :--- |
| A | B | A \|\| B |
| true | true | true |
| true | false | true |
| false | true | true |
| false | false | false |

