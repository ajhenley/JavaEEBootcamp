# A first look at arrays

An array is a container object that holds a fixed number of values of a single type. An array can hold any type of object: integers, numbers, Strings, and even those we haven't learned about yet.

The size \(called length\) of an array is established when the array is created. After creation, its length is fixed.

* The first item of an array has an index value of 0
* The length of an array is equal to the number of elements in the array
* The last item of an array has an index value of one less than the number of elements
* An array's length is fixed. You can change the value of the items but you can't add any new items
* All items in the array have the same data type that was declared when the array was created

## How to declare an array

Arrays are declared by stating the type of element the array will hold. The array can hold either primitives or objects.

```java
double[] temperatures;
String[] args;
```

Note: it is legal to say `String args[]` but ```String[] args`` is more readable and preferred.

After you declare the array you need to construct the array and assign it to the variable you just declared.

```java
temperatures = new double[15];
```

Now you have an array of temperatures that can hold 15 values. Once the size of the array has been set to hold 15 values it will never, ever be able to hold 16 or more values.

But there are no values in your array - yet. It has just been declared. Like your apartment before you move in. It's painted and ready for you but nobody lives there yet.

## Let's move in....

Initializing an array means assigning values to each element. The values can be either primitive values as we're using here or objects which we'll see later. Recall that the indices of your array always start at 0. So to assign a value of 20.0 to the first element you will write: `temperatures[0] = 20.0;` and to assign a value of 90.0 to the last element: `temperatures[14] = 90.0;` If you try to access an element for which you haven't assigned a value you'll get an error.

## How do you access the elements?

Let's print the first element of our array above: `System.out.println(The first element is " + temperatures[0]);`. This will print: `The first element is 20.0`.

That should be enough talk about arrays... let's look at some things we can do with them.

## Things we can do with arrays

```java
import java.util.Random;

public class ArrayDemo {

    public static void main(String[] args) {
        Random rnd = new Random();
        int randomInt;

        //Declare array to hold ten test scores
        int scores[] = new int[10];
        //Initialize elements of an array
        for (int i = 0; i < 10; i++){
            randomInt = 1 + rnd.nextInt(100);
            scores[i] = randomInt;
        }
        //Print the elements of an array
        for (int i = 0; i < 10; i++){
            System.out.printf("Element # %d value is %d\n", i, scores[i]);
        }
        //print the fifth element
        System.out.println("The fifth value is " + scores[4]);
        //Print every other element
        for (int i = 0; i < 10; i+=2){
            System.out.printf("Score %s is %d\n", i, scores[i]);
        }
        //Print the number of elements
        System.out.println("The array length is " + scores.length);
        //Change an element
        scores[0] = 100;
        System.out.println("The first element is now 100");

        //this line will generate an ArrayIndexOutOfBoundsException
        System.out.println(scores[10]);
    }
}
```

