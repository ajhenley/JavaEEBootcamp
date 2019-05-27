# What is an IPO diagram?

An IPO diagram shows the Inputs, Processing Steps and Outputs for a system and is used to describe the structure of a process.The input-process-output \(IPO\) diagram is widely-used in systems analysis and software engineering.

The inputs generally come from the user via the keyboard. They can also come from a file. The processing steps are the steps for your algorithm. The outputs are the results shown to the user on the screen or paper. Outputs can also be written to a file.

## An IPO diagram

To help you develop an understanding of a problem you should read the problem statement. You may need to ask follow-up questions before proceeding. Next, divide the problem into its components.

The solution is often to take the inputs, apply your algorithm and generate the output.

You can document this thought process in an input/output diagram or, Systems Diagram.

### Divide the problem into three components:

* Input – a list of the source data provided to the problem
* Output – a list of the outputs required
* Processing – a list of actions needed to produce the required outputs. This is also your algorithm!

| Input | Processing | Output |
| :--- | :--- | :--- |
| statementBalance | receive statementBalance |  |
| depositsInTransit | receive depositsInTransit |  |
| checksOutstanding | receive checksOutstanding |  |
| bankFees | receive bankFees |  |
| checkbookBalance | receive checkbookBalance |  |
|  | Add statementBalance to depositsInTransit Subtract checksOutstanding from above total subtract bankFees from checkbookBalance |  |
|  |  | Display message indicating if your checkbook is balanced or not |

