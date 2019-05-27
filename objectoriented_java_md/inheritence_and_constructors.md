# Inheritence and constructors

## Inheritence and constructors

* Every class \(including abstract classes\) must have a constructor.
* If you don't type the constructor, Java will create one for you
* You do not call a constructor. It runs when you use the keyword `new`
* Constructors do not have return types; they are not methods
* It's common to have a no-argument constructor
* You can also create a constructor that takes parameters

## What if I don't create a constructor?

You'll get one anyway. Subclasses receive a default constructor that contains a call to the superclass's constructor. If you don't program this then Java will.

## Example 1: Default constructor

**The super call must be the first statement in the constructor.**

## Example 2: A constructor that takes arguments replaces the default constructor.

`Employee(int)` replaces the default `Employee()`.

The subclasses' default constructors are now trying to call a non-existent default Employee constructor.

super\(parameters\);

## Do constructors get inherited?

Constructors are not inherited. If we add a constructor to the Employee class, our subclasses do not compile. The error:

```text
Lawyer.java:2: cannot find symbol
symbol  : constructor Employee()
location: class Employee
public class Lawyer extends Employee {
       ^
```

The short explanation: **Subclasses don't inherit the overridden constructors**. Once you write a constructor that requires parameters in the superclass, you must now write constructors for your subclasses as well.

Subclasses don't inherit the Employee\(int\) constructor.

