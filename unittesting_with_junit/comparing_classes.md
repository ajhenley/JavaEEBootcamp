# Comparing classes

## Comparing strings

Why does `StringA == StringB` always return false?

Comparing strings is not as easy as it may first seem. Be aware of what you are doing when comparing String's using ==.

The difference between the above and below code is that the above code checks to see if the String's are the same objects in memory which they are. This is as a result of the fact that String's are stored in a place in memory called the String Constant Pool. If the new keyword is not explicitly used when creating the String it checks to see if it already exists in the Pool and uses the existing one. If it does not exist, a new Object is created. This is what allows Strings to be immutable in Java. To test for equality, use the equals\(Object\) method inherited by every class and defined by String to return true if and only if the object passed in is a String contains the exact same data:

