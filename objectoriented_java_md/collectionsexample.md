# Collections Example

## Collections Example

## Overview of Collections

The Java Collections API are a set of classes and interfaces. They make it easy to work with collections of objects. They work like arrays with superpowers. Their size can change dynamically, and they have more advanced behavior than arrays.

Collections come in four basic flavors:

* **Lists** contain lists of things
* **Sets** contain unique things
* **Maps** contain unique ID for each thing
* **Queues** contains things arranged in the order they are to be processed

A collection — sometimes called a container — is an object that groups elements into a single variable. Collections allow you to store, retrieve and manipulate data. They represent data items that form a natural group. Examples include a poker hand \(collection of cards\), a mail folder \(letters\), or a telephone directory \(names and phone numbers\).

To use collections in your class you must import the appropriate libraries from the Java API. In this example we will be working with an `ArrayList`.

When you declare your ArrayList as Double then _every object in the list must contain the same data type_, in this case, Double. You can not store primitives in the collection. You can use their object data types. Please only store one type of object in a collection. It will simplify your life. While it would be technically legal to have a collection of type Object it would potentially create a mess. Do so and you may find yourself alone and paying your own way at happy hour.

Adding items to your ArrayList is simple and fun with the add method.

You can print the temperatureList by passing it to our old friend, println:

It will print as follows:

```text
[40.5, 33.9, 37.8, 15.3, 25.6]
```

This doesn't give you much flexibilty so you might prefer to print with an enhanced for loop.

### Sorting

You won't find a sort method in the ArrayList. That's because the ArrayList doesn't give you a way to sort its contents. The `java.util.Collections` class contains a sort method. You can sort your list in ascending order according to the natural ordering. Here's how to use it:

### Finding

You can search for a temperature from list. If the temperature is found then the index will be a positive number equal to the index of your item. If the temperature is not found then the index will be a number equal to the index of where the compiler would expect to find it but multiplied by -1. So, a positive number \(or zero\) means your element was found. A negative number means it was not found.

### Mixing things up

You can also shuffle your collection:

