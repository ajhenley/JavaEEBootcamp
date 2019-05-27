# Developing an Algorithm

> IF THE ALGORITHM IS NOT CORRECT, THE PROGRAM NEVER WILL BE

### Defining the Problem

To help with the initial analysis, the problem should be divided into three separate components:

1. **Input**: a list of the source data provided to the problem.
2. **Output**: a list of the outputs required.
3. **Processing Steps**: a list of the actions needed to produce the required outputs.

When dividing a problem into its three different components, you should simply analyze the actual words used in the specification, and divide them into those that are descriptive and those that imply actions. 

 In some programming problems, the inputs, processes and outputs may not be clearly defined. 

 In such cases, it is best to concentrate on the required outputs which will lead to the required inputs needed to produce the desired output.

 The nouns and their associated adjectives will determine the inputs and outputs.

 The verbs will determine the processing requirements.

We recommend a three column format as below:

| Input | Processing | Output |
| :--- | :--- | :--- |
|  |  |  |

  \#\#\#\#Designing a Solution Algorithm

Designing a solution algorithm is the most challenging task in the life cycle of a program.  Once the problem has been properly defined, you usually begin with a rough sketch of the steps required to solve the problem. The first attempt at designing a particular algorithm usually does not result in a finished product. 

Pseudocode is useful in this trial-and-error process, since it is relatively easy to add, delete or alter an instruction. Note that the algorithm starts with a meaningful name and ends with an **END** statement.

## Checking the Solution Algorithm

 After a solution algorithm has been established, it must be tested for correctness. This step is necessary because most major logic errors occur during the development of the algorithm, and if not detected, these errors can be passed on to the program.  Desk checking involves tracing through the logic of the algorithm with some chosen test data. 

## Selecting Test Data

When selecting test data to desk check an algorithm, you must look at the program specification and choose simple test cases only, **based on the requirements of the specification**, not the algorithm.  By doing this, you will still be able to concentrate on _what_ the program is supposed to do, not _how._ 

## Steps in Desk Checking an Algorithm

By desk checking an algorithm, you are attempting to detect early errors. This process is sometimes called a program walk-through.  It is a good idea for someone other than the author of the solution algorithm to design the test data for the program, as they are not influenced by the program logic. Desk checking will eliminate most errors but is not 100% full proof.

## There are six steps to follow when desk checking an algorithm:

1. Choose simple input test data cases, two or three
2. Determine the expected result for each test case before desk checking your algorithm
3. Make a table of all relevant variables used in the algorithm, variable names at the top of each column
4. Walk the first test case through the algorithm, line by line, keeping a step-by-step record of the contents of each variable
5. Repeat the walk-through process for each of the other test cases.
6. Verify that the expected result from step 2 agrees with the results developed in steps 4 and 5.

If the walk-through results do not agree with the expected results from step 2, revise the algorithm.

