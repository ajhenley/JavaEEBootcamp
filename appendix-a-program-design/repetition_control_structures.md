# Repetition Control Structures

There are three different ways that a set of instructions can be repeated, and each way is determined by where the decision to repeat is placed: 

* at the beginning of the loop \(leading decision loop\)
* at the end of the loop \(trailing decision loop\)
* a counted number of times \(counted loop\)

**Repetition Using the DOWHILE Structure**

The **DOWHILE** construct is a _leading decision loop_ – that is, the condition is tested **before** any statements are executed. 

 General format:

**DOWHILE** condition p is true                  ****

                 Statement block           ****

**ENDDO**              

There are two important considerations about which you must be aware before designing a **DOWHILE** loop.

1. The testing of the condition is at the beginning of the loop.
2. The only way to terminate the loop is to render the **DOWHILE** condition false. 

  \#\#\#\#Using DOWHILE to Repeat a Set of Instructions a Known Number of Times

When a set of instructions is repeated a specific number of times, a counter can be used in pseudocode.

For this construct two actions must be indicated:

1. The counter is initialized before the **DOWHILE** statement and
2. The counter is incremented before the **ENDDO** statement. 

  \#\#\#\#Using DOWHILE to Repeat a Set of Instructions an Unknown Number of Times

Often, a trailer record or sentinel signifies the end of the data. 

This sentinel is a special record or value placed at the end of valid data to signify the end of that data. 

It must contain a value that is clearly distinguishable from the other data to be processed. 

## When a trailer record does not exist – the most common approach

When there is no trailer record to signify the end of the data, the programmer needs to check for an end-of-file marker \(EOF\). 

This EOF marker is added when the file is created, as the last character in the file. 

The check for EOF is positioned in the **DOWHILE** clause, using one of the following equivalent expressions:

**DOWHILE** more data                                                                

**DOWHILE** more records

**DOWHILE** records exist                                                  

**DOWHILE** **NOT EOF**

## Repetition Using the REPEAT…UNTIL Structure

The **REPEAT…UNTIL** structure is similar to the **DOWHILE…ENDDO** structure, in that a group of statements are repeated in accordance with a specified condition. 

However, where the **DOWHILE…ENDDO** structure tests the condition at the beginning of the loop; a **REPEAT…UNTIL** structure tests the condition at the end of the loop. 

The **REPEAT…UNTIL** is a _trailing decision loop_; the statements are executed once before the condition is tested. 

There are two other considerations about which you need to be aware before using **REPEAT…UNTIL**. 

1. **REPEAT…UNTIL** loops are executed when the condition is false; it is only when the condition becomes true that repetition ceases.
2. The statements within a **REPEAT…UNTIL** structure will always be executed at least once. 

###  General formats:

| **REPEAT** |  | **DOUNTIL** condition p is true |
| :--- | :--- | :--- |
|           Statement block | **OR** |     Statement block |
| **UNTIL** condition p is true |  | **ENDDO** |

## Counted Repetition

Counted repetition occurs when the exact number of loop iterations is known in advance. The execution of the loop is controlled by a loop index.

## General format:

**DO** loop-index = initial-value to final-value

          Statement block

**ENDDO**

The DO loop does more than just repeat the statement block. 

* The **DO…ENDDO** loop functions:   ****
* Initializes the “loop-index” to the “initial-value”
* Increments the “loop-index” by 1 for each pass through the loop
* Tests the value of the “loop-index” at the beginning of each pass through the loop to ensure it is in the stated range of values
* Ends the loop when the “loop-index” is greater than the “final-value”

