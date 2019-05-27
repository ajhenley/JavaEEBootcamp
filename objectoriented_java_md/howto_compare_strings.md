# How to compare Strings

## How to compare Strings

`==` tests for reference equality \(whether they are the same object\).

`.equals()` tests for value equality \(whether they are logically "equal"\).

`Object.equals()` checks for nulls before calling .equals\(\) so you don't have to \(available as of JDK7\).

If you want to test whether two strings have the same value you will probably want to use `Objects.equals()`.

```java
// These two have the same value
new String("test").equals("test") // --> true 

// ... but they are not the same object
new String("test") == "test" // --> false 

// ... neither are these
new String("test") == new String("test") // --> false 

// ... but these are because literals are interned by 
// the compiler and thus refer to the same object
"test" == "test" // --> true 

// checks for nulls and calls .equals()
Objects.equals("test", new String("test")) // --> true
Objects.equals(null, "test") // --> false
```

## String Literal Pool

String allocation, like all object allocation, proves costly in both time and memory. The JVM performs some trickery while instantiating string literals. This helps increase performance and decrease memory overhead. To cut down the number of String objects created in the JVM, the String class keeps a pool of strings. Each time your code creates a string literal, the JVM checks the string literal pool first. If the string already exists in the pool, a reference to the pooled instance returns. If the string does not exist in the pool, a new String object is instantiated. It is then placed in the pool. Java can make this optimization since strings are immutable. They can be shared without fear of data corruption.

