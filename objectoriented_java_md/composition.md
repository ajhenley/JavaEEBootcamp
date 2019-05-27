# Composition

## Composition

Complex objects, in real-life\) are often built from smaller, simple objects. A car contains a frame, an engine, tires, a transmission, a steering wheel, and other parts. A personal computer contains a CPU, motherboard, memory, etc... Even you are composed of smaller parts: a head, body, legs, arms, and so on. Composition is process of building complex objects from simple ones. This type of relationship is a containing relationship.

Composition is used for objects that have what we call a **has-a** relationship to each other. A car _has-a_ metal frame, _has-an_ engine, and _has-a_ transmission. A personal computer _has-a_ CPU, a motherboard, and other components. You _have-a_ head, a body, some limbs.

The classes we have used so far have had member variables composed of existing data types \(e.g. int, double, boolean\). This may suffice for designing and implementing small, simple classes. It becomes burdensome for complex classes. Java allows us to build complex classes by using classes as member variables in other classes.

Java composition works by using instance variables that refer to other objects. A Person \(object\) _has a_ Job \(object\). You'll find the Job object as a variable in the Person object below.

Don't worry about the Job object not knowing what Person holds it. The Person object has a Job. That information is available to the program through the Person object. It does not need to go both ways.

Notice that above test program is not affected by any change in the Job object. If you are looking for code reuse and the relationship between two classes is _has-a_ then you should use composition rather than inheritance.

The benefit of using composition is that we can control the visibility of other objects to client classes and reuse only what we need.

Also if there is any change in the other class implementation, for example getSalary returning String, we need to change Person class to accomodate it but client classes don’t need to change.

So composition allows creation of back-end class when it’s needed, for example we can change Person getSalary method to initialize the Job object.

## Your assignment

Create an Education class and make an instance of the Education class a member of the Person class. Your education class should include a list of last 10 schools attended. Create a `toString()` override for both Job and Education that outputs the information in the class to the console. The `toString()` override for Person should use the `toString()` methods for the Job and Education member objects.

