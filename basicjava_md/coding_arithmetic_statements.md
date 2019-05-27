# Coding arithmetic statements

Now that we know how to declare and initialize variables in Java, we can do some mathematics with those variables.

```java
public class DoingMath
{
    public static void main( String[] args )
    {
        int a, b, c, d, e;
        double x, y, z;
        String one, two, red, blue;

        a = 5;
        b = 10;
        c = a + b;
        System.out.println( "a is " + a + ", b is " + b );
        System.out.println( "a + b is " + c );
        d = a - b;
        System.out.println( "a - b is " + d );
        e = a * b;
        System.out.println( "a * b is " + e );
        e = a / b;
        System.out.println( "a / b is " + e );
        e = b / a;
        System.out.println( "b / a is " + e );
        e = a % b;
        System.out.println( "a % b is " + e );
        e = b % a;
        System.out.println( "b % a is " + e );

        x = 1.5;
        System.out.println( "x is " + x );
        y = x * x;
        System.out.println( "x * x is " + y );
        z = b / 3;
        System.out.println( "b / 3 is " + z );
        System.out.println();

        one = "one";
        two = "two";
        red = "red";
        blue = "blue";
        System.out.print( one + " fish " + two + " fish ");
        System.out.println(red + " fish " + blue + " fish");

        // another way to print is...
        // use %s as a placeholder for strings, %d as a placeholder 
        // for integers and %f for floating point decimals
        System.out.printf("%s fish %s fish %s fish %s fish", 
                                            one, two, red, blue);
    }
}
```

## What You Should See

```text
a is 5, b is 10
a + b is 15
a - b is -5
a * b is 50
a / b is 0
b / a is 2
a % b is 5
b % a is 0
x is 1.5
x * x is 2.25
b / 3 is 3.0

one fish two fish red fish blue fish
one fish two fish red fish blue fish
```

The plus sign \(+\) will add integers or doubles together or integers and doubles \(in either order\). The \(+\) sign will concatenate the two Strings together.

The minus sign \(-\) will subtract one number from another. Just like addition, it works with two integers, two doubles, or one integer and one double \(in any order\).

An asterisk \(\*\) is used for multiplication.

A slash \(/\) is used for division. When an integer is divided by another integer the result is also an integer and not a double.

The percent sign \(%\) is used to mean ‘modulus’, which is essentially the remainder left over after dividing.

## Common Student Questions

* Why is 1.1 times 1.1 equal to 1.2100000000000002 instead of just 1.21?

  > Why is 0.333333 + 0.666666 equal to 0.999999 instead of 1.0? Sometimes with math we get repeating decimals, and most computers convert numbers into binary before working with them. It turns out that 1.1 is a repeating decimal in binary.
  >
  >  Remember what I said in the last exercise: the problem with doubles is limited precision. You will mostly be able to ignore that fact in this book, but I would like you to keep in the back of your mind that double variables sometimes give you values that are _slightly_ different than you’d expect. Generally, it is a difference that is washed away by rounding up.

