# What if change activity

The following program is used by your school to process student records. Students enrolled for 12 or more credits are considered fulltime.

## Your Assignment

Change the program so that it only outputs student records for student that are "fulltime".

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
```

