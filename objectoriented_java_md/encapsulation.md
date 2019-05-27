# Encapsulation

Sometimes your class has some internal business to attend to.

For example, your class may contain a method called save which takes as its argument the filename.

The class exposes \(makes available\) the save method.

If you think about it, if your class can save its data to a file, there is a lot happening behind the scenes. Once the user of your class calls the save method your class still has work to do. It must determine if the file exists. If the file doesn't exist then your class must create it on the disk. Then write the data. Finally, close the connection to the file.

> Encapsulation ensures that the user only knows about the save method and not every little detail required to make the save method work.

## Public, Private and Protected, oh my!

Getters/setters allow private member variables to expose their data. A variable not exposed via a getter or setter is effectively hidden \(unless it's declared public which isn't recommended\). Private variables are available for use by the class. If you want a variable to be visible to the class and any future subclasses then declare it as protected. In any event the user has no idea it exists. It's secret to my class.

A variable can have an access modifier **Public** - visible to any class in your program **Private** - visible only to your class \(not sub classes\) **Protected** - visible to your class and any subclasses \(also visible to any classes in the same package\)

You could also have a variable that is available with a getter but has no setter. That would be a read-only variable. A variable with only a setter would be a write-only variable. This isn't common though.

You could also have private variables like counters for use by your class but no other classes. Since there would be no getters/setters for those variables they would be private to the class. Unless you declared them as protected. Then they would be visible to the class and subclasses. But the class/subclass may use them for all kinds of things like database connection information.

So how would the value of a private member variable with no getters or setters get set? If it was database connection information then maybe in the constructor the class could read from a settings file that contained the database settings. This file might be encrypted so it's useless to everyone. But our class may have the decrypt method can read the settings in the constructor to connect to the database.

A lot of the database connection code has been encapsulated in JPA. You set some property values in the settings file. JPA will use that information to connect to your database.

