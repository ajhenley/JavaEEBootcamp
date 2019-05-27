# Shortcut Assignment Activity

The value of a variable can change over time as your program runs. \(It won’t change unless you write code to change it, but it can change is what I’m saying.\)

In fact, this is very common. Something we do often is add a value to a variable. Let’s say the variable x contains the value 10. We want to add 2 to it so that x now contains 12.

We can do this:

This will work but it contains extra steps. We can take advantage of the fact that a variable can contain one value at the beginning of a line of code contain a different value by the end.  
Write something like this:

This also works. That second line says “take the current value of x and add 2 to it. Then store the sum \(12\) into the variable x. So when the second line of code begins executing x is 10, and when it is done executing, x is 12. The order of adding doesn’t matter, so we can even do something like this:

…which is identical to the previous example. Okay, now to the code!

What You Should See

```text
i: 5    j: 5    k: 5
i: 8    j: 2    k: 15

i: 5    j: 5    k: 5
i: 8    j: 2    k: 15

i: 5    j: 5    k: 5
i: 6    j: 3    k: 15

i: 5    j: 5    k: 5
i: 1    j: -2   k: 5

i: 5    j: 5    k: 5
i: 6    j: 4    k: 5
```

Hopefully lines 1-21 are nice and boring. We create three variables, give them values, display them, change their values and print them again. Then starting on line 17 we give the variables the same values they started with and print them.

On line 22 we see something new: a shortcut called a "compound assignment operator." The i += 3 means the same as i = i + 3: "take the current value of i, add 3 to it, and store the result as the new value of i." When we say it out loud, we would say "i plus equals 3."

On line 23 we see -= \("minus equals"\), which subtracts 3 from k, and line 24 demonstrates \*=, which multiplies. There is also /=, which divides whatever variable is on the left-hand side by whatever value the right-hand side ends up equaling. \("Modulus equals" \(%=\) also exists, which sets the variable on the left-hand side equal to whatever the remainder is when its previous value is divided by whatever is on the right. Whew.\)

Then on line 27 I do something else weird. Instead of taking three lines of code to set i, j and k all to 5, I do it in one line. \(Some people don’t approve of this trick, but I think it’s fine in cases like this.\) Line 27 means “Put the value 5 into the variable k. Then take a copy of whatever value is now in k \(5\) and store it into j. Then take a copy of whatever is now in j and store it into i.” So when this line of code is done, all three variables have been changed to equal 5.

Lines 30 through 32 are basically the same as lines 22 through 24 except that we are no longer using 3 as the number to add, subtract or multiply.

Line 38 might look like a typo. If you wrote this in your own code it probably would be. Notice that instead of += I wrote =+. This will compile, but it is not interpreted the way you’d expect. The compiler sees i = +1;, that is, "Set i equal to positive 1." And line 39 is similar "Set j equal to negative 2." So watch for that.

On line 45 we see one more shortcut: the "post-increment operator." i++ just means "add 1 to whatever is in i." It’s the same as writing i = i + 1 or i += 1. Adding 1 to a variable is super common. That’s why there’s a special shortcut for it.

On line 46 we see the "post-decrement operator": j--. It subtracts 1 from the value in j.

Today’s lesson is unusual because these shortcuts are optional. You could write code your whole life and never use them. But most programmers are lazy. They don’t want to type more than they have to. If you ever read other people’s code you will see these often.

## What to do next

Create a application that loops a counter from 1 to 20. Output the count to the console. Only use shortcut assignments. Do not use a For loop.

