# Finding words with the do-while loop

The do-while loop is like the while loop except the expression isn't evaluated until the loop has run at least once. A do-while loop will always run at least one time. Within the loop you need to change the value of the expression or the loop will run forever.

```java
bool run = false;
do {
    System.out.println("This code would run once but that's it.");
} while (run);

run = true;
do {
    System.out.println("This code runs forever - it's an endless loop."); 
} while (run);
```

## Your assignment

We're going to look for a word to see if it is in the UNIX dictionary. Words is a standard file on all UNIX and Linix computers. It is a newline-delimited list of dictionary words. It is often used by spell-checking programs.

The words file is usually stored in `/usr/share/dict/words` or `/usr/dict/words`. If you're using a UNIX or Linux computer then you can refer to the file on your local machine. If you need the file, download it from the following link: [https://users.cs.duke.edu/~ola/ap/linuxwords](https://users.cs.duke.edu/~ola/ap/linuxwords).

Get the words file on your computer. Next create a program that will prompt the user for a word. The program will loop through the file looking for the word. Your program should then tell you that it found the word at position \#xxxx. If the word is not found then the program should display a message. For example: "After checking all 479,829 words the word was not found".

