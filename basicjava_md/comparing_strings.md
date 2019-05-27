# Comparing strings

In Java, `primitiveA == primitiveB` returns true if both primitive variables contain the same value. However, `ObjectA == ObjectB` returns true when both objects share the same **memory location**. It basically boils down to the difference between an object data type and a primitive data type, and we aren't going to cover that until a later chapter. So why am I telling you now? Well, its because Strings are objects not primitives.

## Strings are different

Strings have a built-in method `.equals()` that compares itself to another String. The result is `true` if both strings contain the same content and `false` if they do not. Use the not operator `!` with the `.equals()` method to determine if two Strings are different.

If you test it, you will see that sometimes using == to compare strings gives you predictable results and sometimes it doesn't. Think you can ignore me on this? Do you like to bash your head against the wall while grinding your teeth and wailing uncontrollably? Then **don't EVER use == to compare Strings for equality**. It might actually work sometimes for reasons buried deep inside the internals of Java. But if you value your sanity then use the `.equals()` method to compare Strings. Your head and teeth will thank you.

## Remember this:

The regular relational operators do not work reliably with Strings. They only work on primitives.

## Do this:

Fix the following program so it works. Note: You should be getting comfortable with what a normal java program looks like, so I am not giving you all the code. I just included enough for you to get the idea of the program. It's up to you to provide the rest.

Add a line to print "You should stay inside" if the response is "stormy".

```java
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        System.out.println("How is the weather?");
        String answer = sc.nextLine();

        if (answer == "rain")
            System.out.println("Take your umbrella!");
        else if (answer == "windy")
            System.out.println("Wear your jacket!");
        else if (answer == "snow" )
            System.out.println("Wear a coat and take a shovel!");
        else
            System.out.println("Enjoy your day!");
     }
```

