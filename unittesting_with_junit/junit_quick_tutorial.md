# JUnit Quick Tutorial

## How does JUnit work?

JUnit is a library packed in a jar file. Among other things it contains a tool \(called test runner\) to run your test files. It is not an automated testing tool: you still have to write your test files by hand. JUnit does give you some support so that you can write those test files more conveniently.

Suppose you have a class C that you want to test. We will write the tests in a new class; let’s call it CTest. This CTest is our test file. Actually, test class is a better name. We will typically group the tests in CTest in a bunch of methods called test methods. You will see an example soon.

To actually test C we need to execute its test class C test. This is done by calling JUnit’s test runner tool; we pass the name CTest to it. That’s all. JUnit will then execute CTest for you.

JUnit will report how many of the test methods in C test succeed, and how many fail. The detail of each failure will be reported; this will be in the form of a print of Java’s stack trace leading to the location of the failure.

## How to add JUnit to your project

* Right click on your project and select Build Path. 
* Select Add Libraries. 
* Select JUnit.

## How to create unit tests

* Create a new source folder called UnitTests
* Add your unit tests as a class to that folder.

## The example

We want to test the class below. Why? So when we make changes to it we can verify that our tests still pass. The class is called Avatar. An instance of the Avatar class represents a player in our game. Each player has a name, a birthday, eye color and a gender. Each player probably has other qualities but they're not important for this example.

For example, new Subscription\(1000,2\) will create a new subscription of 1000 cents for the total period of 2 months.

By the way, the class has a number of bugs; e.g. pricePerMonth is supposed to return the price per month in dollars. However it calculates the price in cent.

Let’s write a test

Let us write two simple tests to check if pricePerMonth correctly calculates the price per month:

If we have a subscription of 200 cents for a period of 2 months, its monthly price should be 1 dollar, right? The monthly price is supposed to be rounded up to the nearest cent. So, if we have a subscription of 200 cent for a period of 3 month, its monthly price should be exactly 0.67 dollars. Of course we can write tests without JUnit; but this tutorial is about JUnit. So here is how we write them in JUnit.

Each of the tests above will be implemented as a test method; you then group your test methods in a test class. Usually you would group all the test methods that test a certain target class C is a test class called CTest, but you can also have multiple test classes if you want, and call them whatever you want.

Here is my test class implementing the above two tests:

import org.junit. _; import static org.junit.Assert._ ;

public class SubscriptionTest {

@Test public void test\_returnDollar\(\) { System.out.println\("Test if pricePerMonth returns Dollars..."\) ; Subscription S = new Subscription\(200,2\) ; assertTrue\(S.pricePerMonth\(\) == 1.0\) ; }

@Test public void test\_roundUp\(\) { System.out.println\("Test if pricePerMonth rounds up correctly..."\) ; Subscription S = new Subscription\(200,3\) ; assertTrue\(S.pricePerMonth\(\) == 0.67\) ; } } The marker @Test is called an annotation in Java. When we later execute JUnit’s test runner it needs to know which methods in your test class are test methods \(e.g. you may have several helper methods in your test class\). The @Test is used to mark that a method is a test method.

In the first test \(test\_returnDollar\) we first create a Subscription; we call it S. Then we want to check that S.pricePerMonth\(\) will return the expected value of 1.0. The checking is done by the code:

assertTrue\(S.pricePerMonth\(\) == 1.0\) By the way, the annotation @Test and the method assertTrue are things exported by the JUnit library; so you need the imports as in the above code to use them.

\(Note: some people pointed out that I should not compare a double using == as I did above, due to possible rounding imprecission. However, in this case, the value should exact up to two decimals; so using == is reasonable.\)

Compiling and executing your test

Next we want to execute the above test class \(SubscriptionTest\).

