# What is test coverage?

Coverage works like this: Print your code. Using a highlighter mark all the methods that your unit tests have checked. They're covered. Any methods that are still white aren't covered. Write a test for them.

It's not good enough to have just one test per method. You may need three, five or more. You should test cases of all possibilities. What about the user passing a zero-length password? What about one with a single character? Or starts with a number? Or starts with a space? Or one that's 75 words long? That's five unit tests and we haven't even considered the normal eight character password.

Most people think of full coverage as an insurance policy. It combines their State required liability, Collision and Comprehensive \(vandalism and theft\). But does that cover everything that could happen to your car? What if a flood takes your car for a swim? Or a sinkhole enjoys it for a midnight snack?

Unit tests work the same way. No, you don't pay some Gecko to make cute promises. Unit tests are insurance that your application functions. The more coverage you have the more confident you can be that the application works as expected.

Once your code passes all its unit tests then make sure that no further changes break that. And you'll be on your way to developing robust code.

