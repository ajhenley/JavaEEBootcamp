# Using a Hashmap

A Map cares about unique identifiers. You map a unique key to a specific value. Both the key and the value are objects. A HashMap is an unsorted, unordered Map. When you need a Map and the order of the values is the least of your worldly concerns, the HashMap is here to serve you.

## What can you do with a Hashmap?

* Search for a value based on the key
* Retrieve a collection of just keys or just values
* Add a value to be located by a key
* Delete a value by its corresponding key
* A HashMap can contain one `null` key and any number of `null` values
* If you put a value in a HashMap where a key exists, the old  value is replaced

## How do you declare a HashMap?

The following will create a HashMap called MyMap with the keys as String and the values as String

```java
import java.util.HashMap;
HashMap<String, String> stateCapitals = new HashMap<String, String>();
```

## How do you add values to the HashMap?

```java
MyMap.put("Colorado","Denver");
```

## How do you retrieve the value of a key?

```java
MyMap.get("Colorado");
```

## Here's a complete example

## The output of the above example

```text

A cat says... Meow
A pig says... Oink
A dog says... Woof
A bat says... Squeak
A unicorn says....null
```

