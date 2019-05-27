# Date formatting

Earlier we created our own Date class. But I have news for you. It's already been done. From now on we'll just use the Date classes that are part of the Java API. There are several classes that work together that help us manage dates. Let's look at some of our options now.

Prior to JDK 1.1, the class Date had two additional functions. It allowed the interpretation of dates as year, month, day, hour, minute, and second values. It also allowed the formatting and parsing of date strings. Unfortunately, the API for these functions was not amenable to internationalization. As of JDK 1.1, the Calendar class should be used to convert between dates and time fields and the DateFormat class should be used to format and parse date strings.

The following code will create a Gregorian calendar with a particular date.

* Year must be a four digit integer
* Month is an integer from 0 to 11
* Day must be an integer from 1 to 31

```java
GregorianCalendar gc = new GregorianCalendar(2010,2,15);

System.out.println("Month:" + gc.get(Calendar.MONTH));

//show the month from the array
System.out.println("Month:" + months[gc.get(Calendar.MONTH)]);
System.out.println("Day:" + gc.get(Calendar.DATE));
System.out.println("Year:" + gc.get(Calendar.YEAR));
```

The day of the week is a numeric value from 1 to 7

```java
System.out.print("Day of Week: ");
System.out.println(gc.get(Calendar.DAY_OF_WEEK));
```

&gt; You can display the time if you pass the arguments for hours, minutes, seconds in the call to Gregorian Calendar.

```java
GregorianCalendar gc = new GregorianCalendar(2010,2,15,15,30,0);

System.out.print("Time: ");
System.out.print(gc.get(Calendar.HOUR)+":");
System.out.print(gc.get(Calendar.MINUTE) + ":");
System.out.println(gc.get(Calendar.SECOND));
```

How many days ago was the date?  
 To answer this question, you first get the milliseconds and then convert to the number of days. The number of milliseconds are from January 1, 1970. Java uses this as the epoch, or beginning of time. You can convert this to days as shown below.

```java
 long DateInMS = gc.getTimeInMillis();
```

You can also get this from the Date class The Gregorian Calendar .getTime method returns a date object A date object is also the number of milliseconds since January 1, 1970. The Date class allocates a Date object and initializes it so that it represents the time at which it was allocated, measured to the nearest millisecond.

```java
 Date myDate = gc.getTime();
 myDate.getTime();
```

Once you know the number of milliseconds you can convert them to the number of days

```java
 long millisecondsPerDay = (24*60*60*1000);
 float numberOfDays = DateInMS/millisecondsPerDay;
```

