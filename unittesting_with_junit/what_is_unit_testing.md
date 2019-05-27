# What is unit testing?

As a developer you want to make sure your code works, right? So... create some tests for yourself. Those tests will not become part of the distributed application. Testers in your group have their own testing software. Unit testing is how you, the developer, know your code works. And once written you can check them without much effort.

## Why don't developers make good testers?

Things that seem simple to you are not always simple to your end user. When you test your code and it works that indicates that the code, you wrote as you understood the requirements, works. What if you misunderstood the requirements? Or didn't read them at all?

Testers should be testing the client's requirements. Developers test their interpretations. "Hey, it works on my end!" is not an acceptable response to a client who can't log into the website you just created.

> When should you unit test? Just like voting in Chicago: early and often.

## Unit tests as documentation

Unit tests are the best documentation you could write. A unit test describes how code should work. Unit tests can't get out of date. If you change your code you must change your unit tests or they will fail. Keeps you current, right?

## Unit tests make you a better, faster developer

If you design your application to be testable then you'll design a better application. You won't cram every line of code into main\(\). Instead you'll create testable classes. Be careful not to make every private method public so they can be tested. The private methods will get tested when they are called to help the public methods. They're still testable.

Better yet, if you write the unit tests FIRST then you have a goal. And you'll focus on writing code to pass the unit tests. This encourages you to work faster.

## What should you unit test?

All the public methods in all the classes that you have developed. The private methods are called by the public methods, right? They'll get tested that way. Don't unit test the Java API. It's been done already. It works fine. Your most likely source of errors is your code. Test that. Your tests should cover at least 70% of your code. Less than that means you're not writing enough tests.

## The \#1 reason you should use unit tests

Insurance. Do you need to add a feature? Refactor some code? Allow someone else to modify your application? How do you know if your program still works after the changes have been implemented? If you say anything other than unit testing then you've failed yourself and this course. If the unit tests still pass then your code must still work. A concept so simple a caveman \(who understands computers and Java and modern society\) could understand it.

