# Create a vehicle class

Modify your Car Class application. Now you will create an abstract class for a Vehicle. The Vehicle can run, stop and accelerate. However the abstract class can not fly like a plane or float like a boat. Nor can it haul 10 tons of gravel like the dump truck that just dinged my windshield. Specific implementations are created by inheriting your abstract class.

## How to inherit an abstract class

To inherit your abstract class and all it's methods, etc... use the keyword `extends`. Then create a Plane class, a Boat class and a Car class. Each subclass you create will inherit from the Vehicle class. Any method the vehicle has will be available to the Plane, Boat or Car. Methods you add to the Plane, Boat or Car are specific to that type of Vehicle. For example, you may have a method to make the plane fly which won't be available to the car or boat class \(until next century\).

## Preventing Inheritance

You can make your Plane, Boat and Car implementations final by using the keyword final after the modifier public in the class definition. Final classes can't be inherited. This isn't common but you may sometimes see people do this. Also, you can prevent a specific method from being overridden in the same way.

## An Abstract class

* can not be used to create an object; it must be inherited
* can contain fields, constructors and methods like any other class
* can optionally contain abstract methods

## Abstract Methods

* abstract methods do not have a body \(example shown below\)
* Abstract methods, if any, must be overridden by the subclass. This is also illustrated below.

## Example Abstract Class

## Example subclass for email message

