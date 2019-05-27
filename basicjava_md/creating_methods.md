# Creating methods

A method is a program's way of outsourcing the work to some other block of code.

Water runs out of my sink. The water should go into the drain. The problem is it's getting into the cabinet. I _could_ fix this problem myself but I won't. I'm a programmer. My theory is there's nothing more dangerous than a plumber writing code. The opposite holds as well, I'm sure. I'm not taking chances.

I call Gary and he comes over, fixes it in fifteen minutes and tells me how easy it was. The `MyWifeSaysFixIt` class below doesn't care how the method `callPlumber` works just that it does.

As in life, I couldn't possibly keep track of everything. I don't have all the tools and knowledge to fix my sink, my car, my appliances, etc... and still be a programmer. I outsource some of those things. It makes my life more manageable.

Let's face it. If I tried to fix it then it wouldn't have taken fifteen minutes. And I would have had to call Gary anyway. I've assigned some of my work to Gary. How does this concept work in a program?

```java
public class MyWifeSaysFixIt {

    public static void main(String[] args) 
    {
        boolean isFixed = false;

        // once callPlumber executes, ifFixed doesn't care what happens in
        // the method... it just wants a return value.
        isFixed = callPlumber();

        if (isFixed)
        {
            System.out.println("My wife is happy. The drain is fixed.");
        }else{
            System.out.println("I'm in the doghouse. The drain is leaking.");
        }

    }
    private boolean callPlumber()
    {
        // Some code here where plumber does his thing - I don't even
        // know what he does because I don't have to pay attention
        // I just call him and pay him.

        return true;
    }
}
```

Sometimes you just need to pass the buck. In upcoming topics you'll do just that. And you'll find this makes your code more manageable and easy to follow.

