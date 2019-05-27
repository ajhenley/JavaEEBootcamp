# Inheritance

Let's talk about another key concept from object-oriented programming. Inheritance: Forming new classes based on existing ones.

Inheritence gives us a way to share/reuse code between two or more classes. And code reuse means you don't have to write as much code which means development time is faster. This makes the project manager happy.

Inheritence means there's a parent class being extended. The parent class is called the superclass. We'll also have a child class that inherits behavior from superclass. The child class is called the subclass.

The subclass \(child\) gets a copy of every field and method from superclass \(parent\).

The parent-child have an **is-a relationship**. Every object of the subclass also "is a\(n\)" object of the superclass and can be treated as one. So a car **is a** vehicle.

Suppose we have a class of type Person. Person gets extended to form an Employee. Employee could also be extended to form a Lawyer or an Administrative Assistant. Now we know that a Lawyer is an employee. An Administrative Assistant also is an employee. Each is a Person.

You can only inherit from one class because Java doesn't allow multiple inheritence. But it allows a class to inherit from an entire chain of classes. In fact, all Java classes ultimately inherit from the Object class.

By extending Employee the Lawyer class receives a copy of each method from Employee. The Lawyer can be treated as an Employee by client code. Lawyer can also replace \("override"\) behavior from Employee.

**Override**: To write a new version of a method in a subclass that replaces the superclass's version. No special syntax required to override a superclass method. Just write a new version of it in the subclass.

A subclass can call its parent's method/constructor by preceeding it with the keyword `super`.

A protected field or method is useful for allowing selective access to the inner class implementation. A protected field or method can be seen/called only by:

* the class itself
* its subclasses
* other classes in the same "package" \(packages will be discussed later\)

