# Selection Control Structures

 You can use the selection control structure in pseudocode to illustrate a choice between two or more actions, depending on whether a condition is true or false. 

General Format:

 **IF** \[condition\]

**THEN**

          \[true actions\]

**ELSE**

          \[false actions\]

**ENDIF**

The condition in the **IF** statement is based on a comparison of two items, and is usually expressed with one of the following relational operators:

&lt;   less than                         &gt;       greater than

=   equal to                           &lt;=     less than or equal to

&gt;= greater than or equal to  &lt; &gt;    not equal to

When the condition following the **IF** is true only the actions following the **THEN** and before the **ELSE** are performed.

When the condition following the **IF** is false only the actions following the **ELSE** and before the **ENDIF** are performed.

There are a number of variations of the **IF** statement.

## Simple Selection \(simple IF statement\)

Simple selection occurs when a choice is made between two alternate paths, depending on the result of a condition being true or false. 

 The structure is represented in pseudocode using the keywords **IF, THEN, ELSE** and **ENDIF**. 

Example:

 **IF** Gender = “M”

**THEN**

          Add 1 to Male-Count

**ELSE**

          Add 1 to Female-Count

**ENDIF**

## Simple Selection with Null False Branch \(null ELSE statement\)

 It is used when a task is performed only when a particular condition is true. 

 If the condition is false, then no processing will take place and the **IF** statement will be bypassed.   

The **ELSE** clause is not used. 

Example:

 **IF** Age &gt; 18

**THEN**

          Add 1 to Adult-Count

**ENDIF**

## Combined Selection \(combined IF statement\)

A combined IF statement is one that contains multiple conditions, each connected with the logical operators **AND** or **OR**. 

If the connector **AND** is used to combine two conditions, then **both** conditions must be true for the combined condition to be true. 

If the connector **OR** is used to combine two conditions, then **only one** of the conditions needs to be true for the combined condition to be considered true.

Examples:

```text
IF Gender = "M" THEN
    Add 1 to Male-Count
ELSE
    Add 1 to Female-Count
ENDIF
```

The NOT operator

The **NOT** operator can be used for the logical negation of a condition as follows:

 **IF NOT** \(Record-Code = ’23’\)

**THEN**

          Update customer record

**ENDIF**

## Nested Selection \(nested IF statement\)

 A nested selection occurs when the word **IF** appears more than once within an **IF** statement. 

 A nested **IF** statements can be classified as linear or non-linear. 

## Linear nested IF statements

The linear nested **IF** statement is used when a field is being tested for various values and a different action is to be taken for each value. 

This form of nested **IF** is called linear, because each **ELSE** immediately follows the **IF** condition to which it corresponds. 

| Example: | **Transaction Code** | **Action** |
| :--- | :--- | :--- |
|  | A | Add a new customer record |
|  | C | Change customer record |
|  | D | Delete customer record |
|  | Any other code | Display error message |

**IF** Tran-Code = “A”

**THEN**

          Add a new customer record

**ELSE**

          **IF** Tran-Code = “C”

          **THEN**

                   Change customer record

          **ELSE**

                   **IF** Tran-Code = “D”

                   **THEN**

                             Delete customer record

                   **ELSE**

                             Display error message

                   **ENDIF**

          **ENDIF**

**ENDIF**

## Nested Selection \(nested IF statement\) – continued

 A non-linear nested **IF** occurs when a number of different conditions need to be satisfied before a particular action can occur.  It is termed non-linear because the **ELSE** statement may be separated from the **IF** statement with which it is paired. 

| Example: | **Condition 1** | **Condition 2** | **Action** |
| :--- | :--- | :--- | :--- |
|  | Salaried Employee |  | Pay base salary |
|  | Hourly Employee | Hours &lt;= 40 | Calculate pay at hourly rate |
|  | Hourly Employee | Hours &gt; 40 | Calculate pay with overtime |

**IF** Employee-Code = “H”

**THEN**

          **IF** Hours-Worked &lt;= 40

          **THEN**

                   Calculate pay at hourly rate

          **ELSE**

                   Calculate pay with overtime

          **ENDIF**

**ELSE**

          Pay base salary

**ENDIF**

## **The Case Structure**

 The **CASE** control structure in pseudocode is another way of expressing a linear nested **IF** statement. 

It is used in pseudocode for two reasons:

1. It can be directly translated into many high-level languages, and
2. It makes the pseudocode easier to write and understand. 

Using nested IF statements in pseudocode often look cumbersome and depend on correct structure and indentation for readability. 

## General format:

**CASE OF** variable-name

          **VALUE-1:** statement block-1

          **VALUE-2:** statement block-2

          **VALUE-3:** statement block-3

          **.**

          **.**

          **.**

          **VALUE-n:** statement block-n

          **VALUE-OTHER:** statement block-other

**ENDCASE**

The value of the “variable-name” is compared to each VALUE-n from the top down. When there is an equal condition the corresponding “statement block” is executed. If there is no match the VALUE-OTHER “statement block” is executed.

Example:

|  | **Condition** | **Action** |
| :--- | :--- | :--- |
|  | Age &lt;   3 | Ticket Price =   25% of standard fare |
|  | Age &lt; 13 | Ticket Price =   50% of standard fare |
|  | Age &lt; 20 | Ticket Price = 150% of standard fare |
|  | Age &gt; 64 | Ticket Price =   50% of standard fare |
|  | Other | Ticket Price = 100% of standard fare |

**CASE OF** age

          **&lt;   3:** Calculate Ticket Price =   25% of standard fare

          **&lt; 13:** Calculate Ticket Price =   50% of standard fare

          **&lt; 20:** Calculate Ticket Price = 150% of standard fare

          **&gt; 64:** Calculate Ticket Price =   50% of standard fare

          **VALUE\_OTHER:** Calculate Ticket Price = 100% of standard fare

**ENDCASE**

