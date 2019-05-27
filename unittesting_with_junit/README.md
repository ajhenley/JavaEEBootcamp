# Unit Testing with JUnit

Test-driven development \(TDD\) is a software development process. TDD starts with an \(initially failing\) automated test case. This test case is a Java method which defines a desired improvement or new function. Next, the minimum amount of code is written to pass that test. Finally, the code is refactored to meet acceptable standards.

> "Test-driven development encourages simple designs and inspires confidence".
>
> * Kent Beck, credited with having developed or 'rediscovered' the technique

A 2005 study found that using TDD meant writing more tests. Programmers who wrote more tests tended to be more productive.   
 \([nparc.cisti-icist.nrc-cnrc.gc.ca/npsi/ctrl?action=shwart&index=an&req=5763742&lang=en](http://nparc.cisti-icist.nrc-cnrc.gc.ca/npsi/ctrl?action=shwart&index=an&req=5763742&lang=en)\)

Unit testing is a software testing method by which classes and methods are tested with injected data to determine if they meet the user's requirements.

Ideally, each test case is independent from the others. Substitutes such as method stubs, mock objects,\[5\] fakes, and test harnesses can be used to assist testing a module in isolation. Unit tests are typically written and run by software developers to ensure that code meets its design and behaves as intended.

JUnit is a unit testing framework for Java. JUnit let's you write repeatable tests.

JUnit is a Java library to help you perform unit testing. Unit testing is the process of examining a small "unit" of software \(usually a single class\) to verify that it meets its expectations or specification.

A unit test targets some other "class under test;" for example, the class ArrayIntListTest might be targeting the ArrayIntList as its class under test. A unit test generally consists of various testing methods that each interact with the class under test in some specific way to make sure it works as expected.

JUnit isn't part of the standard Java class libraries. It is included with Eclipse. JUnit can also be downloaded for free from the JUnit web site at [http://junit.org](http://junit.org).

