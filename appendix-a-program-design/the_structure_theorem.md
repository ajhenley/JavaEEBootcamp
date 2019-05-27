# The Structure Theorem

The Structure Theorem states that a solution can consist of a combination of just three constructs. They are sequence, selection and repetition control structures. You can represent each control structure in pseudocode.

## Three control structures

### Sequence

The sequence control structure describes the linear execution of one step after another. A sequence of statements is represented by this construct.

```text
statement a
statement b
statement c
```

A sequence of statements in an algorithm might read:

```text
add 1 to pageCount
Print heading line1
Print heading line2
Set lineCount to zero
Read customer record
```

These instructions illustrate the sequence control structure as a list of steps. Each is written one after the other, from start to finish. Each instruction will be executed as it appears.

### Selection

The selection control structure presents an expression or condition as the choice between two actions. The choice depends on whether the expression evaluates to true or false. This construct represents the decision-making abilities of the computer.

In pseudocode, selection is represented by the keywords IF,THEN,ELSE and ENDIF:

```text
IF condition x is true THEN
    perform statement(s)in the true block
ELSE
    perform statement(s)in the false block
ENDIF
```

If the expression evaluates to true, then the statement\(s\) in the true block will be executed. The statements in the false block will not be executed.

Likewise, if the expression evaluates to false, then the statement\(s\) in false block will be executed and the statement\(s\) in the true block will not be executed.

In either case, control then passes to the next processing step after the delimiter ENDIF.

## A pseudocode example might read:

```text
IF employmentStatus is PART_TIME THEN
    add 1 to partTimeCount
ELSE
    add 1 to fullTimeCount
ENDIF
`
```

### Repetition

The repetition control structure is a list of instructions to be repeated. It is repeated as long as a condition is true. The basic idea of repetitive code is that you execute a block of statements repeatedly. Its execution continues either while a condition is true. This is the sixth basic computer operation, namely to repeat a group of actions.

It is written in pseudocode as:

```text
DOWHILE condition p is true
    statement block
ENDDO
```

The DOWHILE loop is a leading decision loop. That means, the condition is tested before any statements are executed. If the condition is true, the block of statements following that statement is executed once. The delimiter ENDDO then triggers a return of control to the retesting of the condition. If the condition is still true, the statements are executed again. The repetition process continues until the condition is false.

Once control exits the loop, control then passes to the statement that follows the ENDDO statement.It is vital somewhere in the statement block you alter the condition to be false. If not your logic may result in an endless loop. A loop that runs forever.

Here is a pseudocode example that represents the repetition control structure:

```text
Set student_total to zero
DOWHILE student_total < 50
    Read student record
    Print student name, address to report
    add 1 to student_total
ENDDO
```

## This example illustrates a number of points:

* The variable **student\_total** is initialized before the DOWHILE condition is evaluated.
* As long as **student\_total** is less than 50 \(that is, the DOWHILE condition is true\), the statement block will be repeated.
* Each time the statement block is executed,one instruction within that block will cause the variable **student\_total** to be incremented.
* After 50 iterations, **student\_total** will equal 50, which causes the DOWHILE condition to become false and the repetition to cease.
* It is important to realize that the initializing and subsequent incrementing of the variable tested in the condition is an essential feature of the DOWHILE construct.

