# Comparing Objects

Today you're going to learn about comparing people. Yes, despite what your mother may have told you... there are lesser people and greater people. At least in this example.

Let's start with a Person class... to keep our people simple we'll include just the first name and last name. Most people are more complex than that but I'll let you add more features on your own.

Next, try to sort the Person class. Can't do it. It won't work. It's not you. It's me. We're incompatible.

## Why? What can I do? Is there no hope?

The `sort()` method of the Collections class uses `compareTo()` to determine how the LIst or object array should be sorted. There is hope! Simply implement your own `compareTo()` method. Now you get to be the one who determines the criteria by which the classes will sort.

**Here's how to add CompareTo\(\) to the Person class:**

Now you can sort the Person class with `Collections.sort(simpsons);`

## What's next? Can I try it?

You can! Copy the Person class above to a new Eclipse project. Add a field for the person's age. Add the getters and setters as well. Now give each person an age and sort by that age. You are now a sorting genius. Congratulations.

