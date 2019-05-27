# What if

Here is the next Java program you'll enter, which introduces you to the if statement. Type this in, make it run exactly right and then we'll see if your practice has paid off.

The if statement lets us make decisions and control program flow. In the program below, only one line prints but there are 7 `System.out.print` statements. The `if` statement ensures that only the correct one is executed.

## The format of an if statment

```java
if (booleanExpression) {
    System.out.println("This line is inside the if statement");
}else{
    System.out.println("The else block is optional");
    System.out.println("The else block runs if the booleanExpression is false");
}

if (x > 5) {
    y = 3;
    z = 4;
} else {
    y = 4;
    z = 5;
}
```

## When do I need braces in my if statement?

An if statement with only one line of code to run will not require braces```{..}``. However, you must use braces when you want the if statement \(or else clause\) to execute multiple lines of code.

## A bad practice

Can you spot the bad practice below? No, it's not naming your class after a cheesy 1970's song by Bread \(although that shouldn't be permitted\). The bad practice is to not use the braces. Is the intent of the programmer to only change z when x is 7? Use braces to make it clear.

```java
public class IfAPicturePaintsAThousandWords {

    public static void main(String[] args) {
        int x = 4;
        int y = 3;
        int z = 0;

        if (x == 7)
            z = 5;
        y = 6;

        System.out.printf("x = %d, y = %d, z = %d\n",x,y,z);
    }

}
```

## Hurricane wind speed chart

| Category | Wind Speed \(mph\) |
| :--- | :--- |
| 1 | 74 - 95 |
| 2 | 96 - 110 |
| 3 | 111 - 130 |
| 4 | 131 - 155 |
| 5 | 155 and above |

```java
public class Hurricane {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.print("How fast was the wind blowing?" );
        int windSpeed = scan.nextInt();

        // An if statement with only one line of code to run
        // does not require braces
        if (windSpeed <  65) 
            System.out.println("Get over it. That was not a hurricane");
        else if (windSpeed <  96) 
            System.out.println("It was a class 1 hurricane");      
        else if (windSpeed < 111) 
            System.out.println("It was a class 2 hurricane");      
        else if (windSpeed < 131) 
            System.out.println("It was a class 3 hurricane");      
        else if (windSpeed < 155) 
            System.out.println("It was a class 4 hurricane");      
        else {
            // since the else has multiple lines of code to run
            // we use  braces {} to wrap them in a code block
            System.out.println("It was a class 5 hurricane");
            System.out.println("Class 5 is the most severe hurricane");
            System.out.println("Hurricane Katrina was class 5");
        }
    }
}
```

