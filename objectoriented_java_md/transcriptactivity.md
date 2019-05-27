# Transcript Activity

You have written invoice applications that are limited by the fact that you were using arrays to store the data. Now that you have ArrayLists in your toolbelt, you are to write a transcript application that meets the following specifications:

## The Output Should Look Like This

```text

Welcome to the transcript application.

Enter course : java 101
Enter credits:     3
Enter grade:     A
Another course? (y/n): y

Enter product code: english 202
Enter credits:     3
Enter grade:     B
Another course? (y/n): n

Course     Credits     Grade    Quality Points
-------      -----       -----     -----
java  101       3        A        4.0
english 202     3        B        3.0

                                        GPA:  3.5

```

## It must have these classes

| Name | Description |
| :--- | :--- |
| Validator | Provides methods that accept and validate user input. |
| CourseEnrollment | Represents a course enrollment, which includes a course code, credits, and grade. |
| Transcript | Represents a single student's transcript. The course enrollments are represented by an array list. |
| TranscriptApp | Contains the main method for the Transcript application. |

**Transcript Class Information**  
 Constructor  


* Transcript\(\)

Methods  


* void addCourse\(CourseEnrollment courseenrollment\)
* ArrayList getCourses\(\)
* double getOverallGPA\(\)
* String getFormattedGPA\(\)

