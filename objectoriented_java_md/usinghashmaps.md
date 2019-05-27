# Using Hashmaps

## Your Assignment

Create a map to store integers and their word values.  
Prompt user to enter a number and print out the word value.  
If number is not found \(use myMap.containsKey\(10\) then prompt user to add it.

**Example:**

```text

Prompt: Enter a number: 10
Response: You entered ten.
Would you like to try again? (Y/N): Y
Enter a number: 31
I do not know that number. Please tell me:
Thirty-one
Would you like to try again? (y/n):
```

Add the key and value to the map with the following line of code:

```java
myMap.put(10,"ten");
```

Retrieve the value with

```java
//check if the map contains the key
if (map.containsKey(10)){
    System.out.println(myMap.get(10));
}else{
    //write code here to insert the key/value
}
```

