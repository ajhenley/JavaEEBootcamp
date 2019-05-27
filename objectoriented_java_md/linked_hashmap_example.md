# Linked HashMap Example

A `LinkedHashMap` maintains the insertion order. It's slower than the `Hashmap` for adding and removing elements. It's faster than the `HashMap` for iterating through the elements of your collection.

Use the `LinkedHashMap` when the order of insertion is important. For example: showing values in a shopping cart.

`LinkedHashMap` is an implementation of `java.util.Map` interface with predictable iteration order \(the order of insertion\). `LinkedHashMap` will iterate in the order in which the entries were put into the map.

This implementation differs from `HashMap`. It maintains a doubly-linked list running through its entries. This linked list defines the iteration ordering. Items are stored in the order in which keys were inserted into the map. The insertion order is not affected if a key is re-inserted into the map.

The other two important implementations of Map interface are `java.util.HashMap` and `java.util.TreeMap`. They offer mostly the same functionality. The most important difference is the order in which iteration through the entries will happen. `HashMap` makes no guarantee about the order. The order can even change completely when new elements are added. `TreeMap` will iterate according to the “natural ordering” of the keys according to their `compareTo()` method \(or an externally supplied java.util.Comparator\). `LinkedHashMap` will iterate in the order in which the entries were put into the map.

