# Classes and Objects

First there was functional or top-down programming. All programs had a single entry point and worked their way down, line by line, to a single exit point. They could jump around with various routines and go-to statements but all code was basically one large file. And it got cumbersome.

## Division of labor

Somehow the idea emerged that you could have a programmer develop code in units or blocks or what is now known as classes. And these classes could be developed simultaneously and put together in a larger program. And re-used in other programs. And tested independently. Once tested they wouldn't have to be tested again.

## What goes into a class?

Each class should have one purpose. Maybe you need a Calendar class to display calendars and perform date arithmetic. Or an Invoice class to display/print an invoice and perform all the calculations that go with that. Or an Encryption class which can take some text or a file and return an encrypted version of each. Each class can be used to create objects. These will contain the data and any methods to process that data in order to fulfill the purpose of the class.

## Differences between classes and objects

The class is the code that will be executed, the type of data to be saved and the way it interacts with other things. The object is a particular instance of an object.

## What happens in Vegas \(my class\) stays in Vegas \(my class\)

Encapsulation is the idea that your class is a black box. When we say something is a black box, that means that goes on inside the object doesn't matter to the user. You just need to interact with the class through its interface.

## The interface I show the world

The interface is those methods which are publicly available for use by other programmers.

## Extending classes with inheritance

A more generalized class like Animal can be extended to a more specialized class like cow, bird and fish. All the features of Animal are the same amongst different species. But cows, birds and fish have their own specialized methods. One can give milk, the other can fly and the other can swim. Finally, keep in mind that all cows are animals but not all animals are cows.

