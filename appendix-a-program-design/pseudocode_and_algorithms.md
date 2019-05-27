# Pseudocode and Algorithms

## Algorithm

An algorithm represents the ordered sequence of steps required to solve a problem. Following the steps will always result in the solution. When a computer is to solve a particular problem, the steps to the solution get communicated to the computer. This makes the study of algorithms an important part of computer science.

The algorithm gets translated to a programming language, such as Java. The Java compiler will translate the program into instructions the computer can execute. This produces the required output from the given input.

But translating the algorithm to computer code is not straight forward. To simplify the process, translate the algorithm into pseudocode. The pseudocode will then more easily translate into Java or another programming language.

## Pseudocode

Pseudocode is a human-readable representation of an algorithm. It is not written the specific syntax of any particular programming language. However, a programmer can easily translate pseudocode to Java because the pseudocode is the algorithm plus any considerations for making it into a program.

There is not a standard format for pseudocode. It tends to be a cross between some of the more widely used programming languages and natural language. Pseudocode can generally be read by programmers who are familiar with different programming languages.

Pseudocode allows one to include all the constructs of the Structure Theorem. Pseudocode can include sequence, selection and repetition as needed to perform the algorithm.

## Pseudocode Conventions

* Statements are written in simple English.
* Each instruction is written on a separate line.
* Keywords and indentation are used to signify particular control structures.
* Each set of instructions is written from top to bottom, with only one entry point and one exit point.
* Groups of statements may be grouped into named modules.

## So what's the difference?

An algorithm is the solution to the problem. It presents a well defined sequence of steps that provides a solution for a given problem. Pseudocode represents the algorithm in a format that resembles any programming language. Pseudocode is the algorithm written in terms of the Structure Theorem.

The client or business analyst derive the algorithm. Someone with knowledge of programming derives the pseudocode. The programmer develops the program from the pseudocode. The compiler translates the program into byte code or machine code and the program runs! The client is happy. And the Project Manager takes all the credit.

## Finally! The example:

### Algorithm:

Our local weatherperson tells us how to convert a temperature from Fahrenheit to Celsius. She says to subtract 32 from the Fahrenheit temperature and then multiply that value by 5/9. That's the algorithm.

From that we derive the pseudocode:

```text
Prompt user for fahreheitTemp 
Get fahreheitTemp
Calculate celciusTemp = (fahreheitTemp &ndash; 32) * 5/9
Display celciusTemp
```

Which description would you rather have in front of you when you're ready to write a program to convert temperatures? The algorithm or the pseudocode?

Notice that the pseudocode example has made several decisions for the programmer. These include the order of operations, the variable names and the steps to follow.

The programmer can now focus on programming and not the business problem.

Programmers are often asked to develop solutions for problems they do not fully understand. It is unlikely that you are a meteorologist. You wouldn't need to be because that person already figured out the formula and gave you the algorithm. You just have to program it. And the project manager has already told the client you did that yesterday.

