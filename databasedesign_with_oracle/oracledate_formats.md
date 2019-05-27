# Oracle Date Formats

The Oracle `TO_DATE()` function will convert either a character string or an expression into a date value.

**Example Syntax**  
These all show valid date formats for "February 16th, 2009":

```sql
to_date('16-Feb-09', 'DD-Mon-YY')

to_date('02/16/09', 'MM/DD/YY')

to_date('021609', 'MMDDYY')

to_date('16-Feb-09', 'DD-Mon-YY HH:MI:SS') 

to_date('Feb/16/09', 'Mon/DD/YY HH:MI:SS')

to_date('February.16.2009', 'Month.DD.YYYY HH:MI:SS')
```

The 'format' string must be a valid DATE format:

```sql
YYYY=year 
MM=month
DD=Day
HH=Hour
Mi=Minute
```

If no format is specified Oracle will assume the default date format has been supplied in char.

## Converting Dates to Strings

The Oracle `to_char()` SQL function is used to transform a DATE or NUMBER datatype into a displayable text string.

```sql
to_char(number_type, format_mask)
```

Examples of the Oracle SQL to\_char function might include:

```sql
to_char(sum(decode(substr(time,10,2),'23',1,0)),'99')
to_char(sn.begin_interval_time,'hh24')
TO_CHAR(BID.START_DATE, 'dd mon yyyy') || ' to ' || TO_CHAR(BID.END_DATE, 'dd mon yyyy')
to_char(begin_interval_time,'yyyy-mm-dd hh24:mi')
TO_CHAR( COLUMN_NAME,'DD-MON-RRRR HH24:MI:SS' )

SELECT TO_CHAR(SYSDATE,'dd-Mon-yyyy hh:mi:ss PM') FROM dual;
```

## Format Specifiers

| **Code** | **Description** |
| :--- | :--- |
| D | Day of the week |
| DD | Day of the month |
| DDD | Numerical day of the year, 1 ~ 365 \(366 for Leap years\) |
| DAY | Full textual representation of the day, i.e. "Monday", "Tuesday", "Wednesday" |
| DY | Day in three letters, i.e. "MON", "TUE", "FRI" |
| W | Week of the month |
| WW | Week of the year |
| MM | Month in two digits, i.e. 01 = Jan, 02 = Feb,...12 = -Dec |
| MON | Month in three characters, i.e. "Jan", "Feb", "Apr" |
| MONTH | Full textual representation of the Month, i.e. "January", "February", "April" |
| RM | Month in Roman Characters \(I-XII, I-Jan, II-Feb, ... XII-Dec\) |
| Q | Quarter of the Month |
| YY | Last two digits of the year. |
| YYYY | Full year |
| YEAR | Year in words like "Nineteen Eighty Seven" |
| HH | Hours in 12 hour format |
| HH12 | Hours in 12 hour format |
| HH24 | Hours in 24 hour format \("military time"\) |
| MI | Minutes |
| SS | Seconds |
| FF | Fractional Seconds |
| SSSSS | Milliseconds |
| J | Julian Day i.e Days since 1st-Jan-4712BC to till-date |
| RR | If the year is less than 50 then Oracle considers the year as a 21st century date. If the year is greater than 50 then Oracle considers the year to be in the 20th century. |

