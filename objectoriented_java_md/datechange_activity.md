# Date change activity

The following application is supposed to output just the date on the first line and time on the second. It kinda does it. It kinda doesn't. Change the application to use `DateFormat` and give just the date on the first line and just the time on the second one.

```java
import java.util.Date;

public class DateChangeActivity {

    public static void main(String[] args) {
        Date now = new Date();
        System.out.println(now.toString());
        System.out.println(now.getTime());
    }
}
```

