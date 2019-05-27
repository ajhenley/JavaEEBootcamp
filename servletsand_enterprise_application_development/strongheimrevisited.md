# Strongheim Revisited

It seems that Professor Strongheim can't easily compute GPAs accurately. The professor needs to store the relative weights of the different types of assignments in a database table. This should allow him to change the weights at will and then recompute the grades of his students.

## Example

The following table demonstrates how Professor Strongheim computes his grades. He takes the percentage in each category and multiplies it by its respective weight. The sum of these contributions is the total grade percentage.

```text
homework*(the weight of homework) + 
  quizzes*(the weight of quizzes) + 
      exams*(the weight of exams) = final course grade
```

| Category Name | Percentage in Category | \* | Weight of Category | = | Contribution |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Homework | 89% | \* | .30 | = | 0.267 |
| Quiz/Test | 91% | \* | .50 | = | 0.455 |
| Exam | 85% | \* | .20 | = | 0.170 |
|  |  |  |  | Total 89.2% |  |

## Your Assignment

Change your application to account for the weighted grades as discussed above.

As long as you're making changes allow the application to handle students in different classes. Some students in Professor Strongheim's 9:30 Earth Science class are also in his 1 pm Intro to Physics class. You need to ensure the Professor doesn't mix the grades between those two classes.

