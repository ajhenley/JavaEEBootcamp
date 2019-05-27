# Deep thoughts random activity

Most of the life of a program is spent in maintenance. Consequently, most of the life of a programmer is spent maintaining existing programs.

Your job now is to change the following application. The first step is to copy the code to Eclipse and get it running. You'll see that the program asks the user for their goal and prints out a motivational response. Then it exits.

There aren't enough responses. Add five more. You can make them up or you can search online for ideas. Change the code so that it picks a random number from 1-20 and add your responses.

We'd like to apply what we know about classes to reduce the code in `main()`. Then we can take advantage of object-oriented design. You should create a class called DeepThoughts which simply returns a random inspirational quote. The class needs a method to generates the random quote. Implement the DeepThoughts class in your main method as follows:

`response = DeepThoughts.inspireMe();`

We've already learned about while loops. A while loop would to allow the user to receive another quote or exit. Add a while loop to the program so the user is continually prompted to either get a quote or exit. That way the user could have lots of goals.

