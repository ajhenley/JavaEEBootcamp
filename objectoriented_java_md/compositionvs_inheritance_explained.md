# Composition vs Inheritance Explained

## Composition vs Inheritance Explained

Both composition and inheritance enable a class to reuse the code of another class. Programmers may use inheritance to get one class to contain the functionality of another. Sometimes that's the best idea in the world. Sometimes it's a square wheel. Which to use and when? The correct answer depends on the relationship between the classes.

With _Composition_ you learned how a Person class could have a Job. Or an Education class could contain schools. We call these _has-a_ relationships because the first class _has-an_ object of the second class.

_Inheritance_ is the other type of relationship. It occurs when one class inherits another. An Employee class is a more specific instance of a Person. It inherits the Person class. This type of relationship is called an _is-a_ relationship. All the attributes of Person are in Employee as well as some attributes specific to Employees. Such as Department, JobTitle, PayRate, etc...

## How to implement Inheritence

Here's an example with an Instrument and a Saxophone. Notice that the Instrument does not know anything about the Saxophone. The Instrument is a class that existed when the developer discovered the need for a more specific instrument. Good coding practice says we don't want to modify working code. We should extend it.

## What You Should Do Now

Create an Employee class and make it extend the Person class. Your employee class should include fields for Department, JobTitle and PayRate. Create a `toString()` override for both Job and Education that outputs the information in the class to the console. The `toString()` override for Person should use the `toString()` methods for the Job and Education member objects.

