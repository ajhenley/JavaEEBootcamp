# Formatting prices with two decimal places

## Formatting prices with two decimals

The **NumberFormat** class helps you to format and parse numbers or currency values. Since it's an abstract class you must call the `getInstance()` method or some variation of that method.

```java
myString = NumberFormat.getInstance().format(myNumber);
```

## Formatting prices with two decimal places

You can use the NumberFormat class from the Java API

```java
NumberFormat nf = NumberFormat.getInstance();
nf.setMaximumFractionDigits(2);
nf.setMinimumFractionDigits(2);
setRoundingMode(RoundingMode.HALF_UP);

System.out.print(nf.format(decimalNumber));
```

Or you can use String.format. This will also work with printf to print a formatted string.

```java
double myDouble = 3.5;
String formattedData = String.format("%.02f",myDouble);
```

