# Measuring Complexity

## When is Efficiency Important?

Not every problem requires the most efficient solution available. For our purposes, the term efficient is concerned with the time and/or space needed to perform the task. When either time or space is abundant and cheap, it may not be worth it to pay a programmer to spend a day or so working to make a program faster.

However, here are some cases where efficiency matters:

* When resources are limited, a change in algorithms could create great savings and allow limited machines \(like cell phones, embedded systems, and sensor networks\) to be stretched to the frontier of possibility.
* When the data is large a more efficient solution can mean the difference between a task finishing in two days versus two weeks. Examples include physics, genetics, web searches, massive online stores, and network traffic analysis.
* Real time applications: the term "real time applications" actually refers to computations that give time guarantees, versus meaning "fast." However, the quality can be increased further by choosing the appropriate algorithm.
* Computationally expensive jobs, like fluid dynamics, partial differential equations, VLSI design, and cryptanalysis can sometimes only be considered when the solution is found efficiently enough.
* When a subroutine is common and frequently used, time spent on a more efficient implementation can result in benefits for every application that uses the subroutine. Examples include sorting, searching, pseudorandom number generation, kernel operations \(not to be confused with the operating system kernel\), database queries, and graphics.

In short, it's important to save time when you do not have any time to spare.

When is efficiency unimportant? Examples of these cases include prototypes that are used only a few times, cases where the input is small, when simplicity and ease of maintenance is more important, when the area concerned is not the bottle neck, or when there's another process or area in the code that would benefit far more from efficient design and attention to the algorithm\(s\).

## Big-O notation

Big O notation is a method of expressing the complexity of an algorithm. But how does it work? It’s one of those things that sounds more complex than it really is. Let’s build up to it. I'll be using Python 3 for my examples. Idea 1: The easiest way to measure the execution time of a program across platforms is to count the measure of steps. def once\(word\): print\(word\)

def many\(word\): for i in range\(100\): print\(word\) Without knowing anything about the computers involved, it’s obvious which of the above programs will run faster. This also shows that number of steps does not equal lines of code. Idea 2: You can represent the number of steps with algebra. For the two examples above, the number of steps are 1 and 100. But what if it runs a variable amount of time?

```text
def show(n)
    for i in range(n):
        print(‘Word’)
The function above will run n times. There can also be powers of n, such as:
def squared(n):
    for i in range(n):
        for j in range(n):
            print(‘Word’)
The function above will run in n2 time.

def show(n):
    for i in range(n):
        for j in range(n):
            print(‘Word’)
    for k in range(n):
        print(‘Word’)
        print(‘Word’)
```

This function will run in n2 + 2n time.

Idea 3: The most critical part of the representation is the greatest power of n. Consider 3n + 5. As n increases in value, the 5 part becomes less and less important. 100005 is pretty close to 100000. The same can be said of the 3 in the equation. In the case of n2 + n, the lone n becomes less important. Big O notation is the logical continuation of these three ideas. The number of steps is converted to a formula, then only the highest power of n is used to represent the entire algorithm.

```
 def multi(n): for i in n: print(n) print(‘Word’) There are 2n steps. Runs in O(n) time. def squared(n): for i in n: for j in n: print(n) for i in n: print(n) There are n2 + n steps. Runs in O(n2 ) time. def show(n): print(n) print(n) print(n) 
```

