# Exceptions

## What is an exception?

Definition: An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions. Short answer: It's an error!

## So what am I supposed to do about it?

You have two choices. Handle it or throw it up the call stack. We'll talk more about the call stack later. For now know that the call stack is a running list of the methods that have been called by your program. As each method finishes, control returns to the previous method.

After your method throws an exception, Java looks for someone to handle it. If you've written code that can handle it, great! You're talking to the manager on duty. Otherwise the exception says to your method: "I want to talk to the supervisor!". Put your ear to your computer. It literally says that.

So the method that called your method gets the error. Can that method handle it? No? The exception goes up the call stack. Somebody is going to handle this error. Or this program will crash. And heads will roll.

Let's first look at some code that handles the exception on its own. This is easy - just surround the code that _could_ cause an error with try..catch statements.

In the following code, we its possible that the file doesn't exist or isn't available. Since it is likely we give the user a "nice" message instead of crashing abruptly when it happens. Notice that we can have as many catch clauses as we like. We simply list them in order of most specific exception to most general exception.

```java
import java.io.*;
public class ExceptionExample {
//second commit
    public static void main(String[] args) {
        FileInputStream fis = null;
        int k;

        try
        {
            fis = new FileInputStream("c:\\myfile.txt");

            while ( (k = fis.read()) != -1)
            {
                System.out.println((char)k);
            }
        //catch the most specific exception first    
        }catch (FileNotFoundException e)
        {
            System.out.println("There is no file!");
        //an IO exception is more general... maybe the drive is corrupt
        }catch (IOException e)
        {
            System.out.println("There is an IO exception.");
        //This catches all the other exceptions that we can catch
        //So save the more general exception for last
        }catch (Exception e)
        {
            System.out.println("Something else went wrong");
        }
    }
}
```

There's one more thing I want to tell you, that you can do with exceptions: You can give them away.

I can show this by rewriting the above example with multiple methods. Then we'll pass the exception from one method to another to another until it is handled.

```java
import java.io.*;
public class ExceptionDemo {
//second commit
    public static void main(String[] args) {
        MethodA();
    }
    private static void MethodA(){
        MethodB();
    }
    private static void MethodB(){
        try{
            MethodC();
        }catch(FileNotFoundException e){
            System.out.println("File not found. You'll find it in the last place you look.");
        }catch(IOException e){
            System.out.println("IO Exception occurred. Bummer!");
        }
    }
    private static void MethodC() throws FileNotFoundException,IOException{
        FileInputStream fis = null;
        int k;
        fis = new FileInputStream("myfile.txt");
            while ( (k = fis.read()) != -1)
            {
                System.out.println((char)k);
            }
            }
}
```

## Finally

You can add a finally clause to a try-catch block. The code inside the finally clause will always be executed, even if an error is found. If your code has a return statement inside the try or catch block, the code inside the finally-block will get executed before returning from the method.

The finally clause allows you to ensure that open files, open database connections or other resources are closed or freed.

```java
FileInputStream fis = null;
        try{        
                int k;
                fis = new FileInputStream("myfile.txt");
                    while ( (k = fis.read()) != -1)
                    {
                        System.out.println((char)k);
                    }
        }catch(FileNotFoundException e){
            System.out.println("File not found. You'll find it in the last place you look.");
        }catch(IOException e){
            System.out.println("IO Exception occurred. Bummer!");
        }finally{
            try {
                fis.close();
            } catch (IOException e) {
                System.out.println("We *still* have an IO error!");
            }
        }
```

