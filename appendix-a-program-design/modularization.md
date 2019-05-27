# Modularization

Modular programming occurs when you organize your program\(or algorithm\) into separate modules. Modularization makes your program collection of independent, reusable components. The process reduces redundant code. Each component contains just the code to perform its specific functionality. Each method of each module can be independently tested/verified with unit tests.

When creating programs in Java modules will become either methods, classes or packages. A method, sometimes called a function, is a unit of code that performs one task. A method in Java will never exist outside of a class. A class generally contains fields and methods modeled after the behavior of an object. A package is a collection of related classes.

## The Modularization Process

Write down the tasks or processing steps which solve your problem. Some tasks may naturally belong together and could be candidates for inclusion in a module.

It should have a single entry, and a single exit with a top-to-bottom sequence of instructions.The name of the module should describe the work to be done as a single specific function.

Name each module by using a verb, followed by a one or two-word object. One module can call or evoke another module.

This passes control the called module. When the called module terminates control is passed back to the calling module.

## The Main Routine - your starting point

The main routine is the starting point for your program. The main routine ties all the modules together and coordinates their activity. The main routine contains the main processing functions, and the order in which they will execute. It also shows the flow of data and the major control structures. The main program should be easy to read, be of manageable length and show the logic structure of the program.

The signature of the main routine in a Java program is:  
 `public static void main(String args[])`

## Benefits of Modular Design

* Logical organization – each module performs only one function
* Code Reuse – the methods in your module can be used by other modules
* Elimination of redundancy – no need to repeat writing the same code
* Maintenance – changes to one module should not impact other modules
* Ease of testing – unit tests can confirm the functionality of each method in your module.

## Side Note:

Java doesn't yet contain the concept of a module. This is proposed for a future release. A module would be a collection of Java Archives \(JARs\) the purpose of which would be to handle versioning issues.

The proposed specification change would be a ... "distribution format \(i.e., a Java module\) and its metadata as a unit of delivery for packaging collections of Java code and related resources. The metadata would contain information about a module, the resources within the module, and its dependencies upon other modules. The metadata would also include an export list to restrict resources from being exposed outside the module unintentionally. The metadata may allow subset of exposed resources to be used by other modules selectively."

Apparently the issues they're trying to resolve are: 1. Version conflicts with updated dependencies. 2. No uniform deployment model for Java application and extensions. 3. No means to share Java extensions among different JREs on the same system.

