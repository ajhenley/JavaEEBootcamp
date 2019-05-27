# Submit your answers to Randomness

* Delete the `1 +` in front of all six lines that pick numbers 1-5, so that they look like this: `System.out.print( r.nextInt(5) + " " );` Run the program a few times, and see if you can figure out what range the new random numbers are in.
* Change the `1 +` in front of all six lines that pick numbers 1-5, so that they look like this: `System.out.print( 3 + r.nextInt(5) + " " );` Run the program a few times. Is it picking random numbers from 3 to 5? If not, what range are they?
* Change the line where you create the random number generator so that it looks like this: `Random r = new Random(12353);` This number is called a seed. Run the program a few times. What do you notice? What happened to the random numbers?
* Change to random seed to something else and observe the behavior. What happens to the random numbers?
* Create an array of 10 elements. Select each element randomly. Modify the array to count the number of times each element is used.

