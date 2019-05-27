# Data types in the database

| Category | Description |
| :--- | :--- |
| Character | Strings of characters |
| Numeric | Integer, decimal and floating-point numbers |
| Temporal | Dates and times |
| Large object \(LOB\) | Text, images and files |
| Rowid | Address for each row in the database |

## Storing text

`char(n)` - stores a fixed-length string of n characters. The size \(optional\) of n can be from 1 to 2000. `varchar2(size n)` - stores a variable length string of characer data up to 4000 characters. Size is required.

## Storing numbers

`number(p,s)` - stores negative and positive numbers. Precision\(p\) can range from 1 to 38. scale \(s\) can range from -84 to 127. The precision indicates the number of digits that can be stored. The scale indicates the number of decimal digits that can be stored to the right of the decimal point.

## Storing Dates

`date` - stores data and time information in a fixed length. Stores century, year, month, day, minute, hour, and second. Does not store time zone. `timestamp(fsp)` - Extends date to include the fractional part of a second where the fractional second precision \(fsp\) is the number of decimal places used to store the fractional part of a second.

## Boolean data

Oracle doesn't have a data type called boolean for storing true/false or yes/no values. Programmers will often create a field that is of type char and use 'Y' for yes or 'N' for no. You'll also see people use the value of 0 for No or False and 1 for Yes or true. This is recommended because it will interact correctly with JDBC and other programming environments. Also, the char data type consumes less space in the database than Number.

## Try it yourself

```sql
create table tblBoolean (bool char check (bool in (0,1));
insert tblBoolean tbool values(0);
insert into tblBoolean values(1);
```

## Converting data

`to_char(expr,fmt)` will convert the expression expr to varchar2 with an optional format specifier, fmt `to_number(expr,fmt)` will convert the expression expr to number type with an optional format specifier, fmt `to_date(expr, fmt)` will convert the expression expr to date type with an optional format specifier, fmt

## Oracle to\_date format specifier

You can put these together in a string as follows: `SELECT TO_DATE('2012-06-05', 'YYYY-MM-DD') FROM dual;`

| format specifier | description |
| :--- | :--- |
| YYYY | 4-digit year |
| YY | 2-digit year |
| RRRR | 4-digit or 2-digit year, 20th century used for years 00-49, otherwise 19th |
| MON | Abbreviated month \(Jan - Dec\) |
| MONTH | Month name \(January - December\) |
| MM | Month \(1 - 12\) |
| DY | Abbreviated day \(Sun - Sat\) |
| DD | Day \(1 - 31\) |
| HH24 | Hour \(0 - 23\) |
| HH or HH12 | Hour \(1 - 12\) |
| MI | Minutes \(0 - 59\) |
| SS | Seconds \(0 - 59\) |

