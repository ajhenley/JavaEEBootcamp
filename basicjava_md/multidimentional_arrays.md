# Multidimensional Arrays

> A multidimensional array is an array whose elements contain another array

An array can not only contain elements but also each element of an array could be ... another array! You've actually seen this. Lots of times, I bet. Have your used a calendar? Have you worked in Excel before? Think of the first array as being the rows. And each row contains an array of columns. If you stored your Student Gradebook in an Excel worksheet you would have an array of records \(each student\) and each student would contain four columns: gender, major, state, average score.

Your array would look like this:

| M | Econ | MD | 99 |
| :--- | :--- | :--- | :--- |
| F | Mktg | VA | 89 |
| F | Biology | NJ | 100 |

_... continues for 97 more rows..._

In Java, you could create this same structure as follows. This allows fast-progarmmatic access to your data using two dimensions. Think of the as the row index \(or the index of the first array\). And the column index \(or the index of the second array\).

You can access the elements of a two-dimensional array with two nested for-loops.

```java
public class MultiDimArrayDemo {
    public static void main(String[] args) {

        //array of gender, major, state, score
        String[][] studentGradebook = new String[100][4];

        studentGradebook[0][0] = "M";
        studentGradebook[0][1] = "Econ";
        studentGradebook[0][2] = "MD";
        studentGradebook[0][3] = "99";

        studentGradebook[1][0] = "F";
        studentGradebook[1][1] = "Mktg";
        studentGradebook[1][2] = "VA";
        studentGradebook[1][3] = "89";

        studentGradebook[2][0] = "F";
        studentGradebook[2][1] = "Biology";
        studentGradebook[2][2] = "NJ";
        studentGradebook[2][3] = "100";

        for (int i = 0; i < 3; i++)
        {
            for (int j = 0; j < 4; j++)
            {
            System.out.println(studentGradebook[i][j]);
            }
        }

    }
}
```

## Your Assignment:

* Create a multidimensional array in Eclipse that prints five rows numbered 1 to 5 and ten columns numbered 1 to 10. Display them as a matrix as shown below. 
* Create an array to display the multiplication tables for the values 1 to 12. Your multiplication tables should display as shown below. The intersection of a row value and a column value would be the product of those two values.

  ```text
  row 0 col 0    row 0 col 1    row 0 col 2    row 0 col 3    row 0 col 4    
  row 1 col 0    row 1 col 1    row 1 col 2    row 1 col 3    row 1 col 4    
  row 2 col 0    row 2 col 1    row 2 col 2    row 2 col 3    row 2 col 4    
  row 3 col 0    row 3 col 1    row 3 col 2    row 3 col 3    row 3 col 4    
  row 4 col 0    row 4 col 1    row 4 col 2    row 4 col 3    row 4 col 4    
  row 5 col 0    row 5 col 1    row 5 col 2    row 5 col 3    row 5 col 4    
  row 6 col 0    row 6 col 1    row 6 col 2    row 6 col 3    row 6 col 4    
  row 7 col 0    row 7 col 1    row 7 col 2    row 7 col 3    row 7 col 4    
  row 8 col 0    row 8 col 1    row 8 col 2    row 8 col 3    row 8 col 4    
  row 9 col 0    row 9 col 1    row 9 col 2    row 9 col 3    row 9 col 4    
  row 10 col 0    row 10 col 1    row 10 col 2    row 10 col 3    row 10 col 4    
  row 11 col 0    row 11 col 1    row 11 col 2    row 11 col 3    row 11 col 4
  ```

```text
1    2    3    4    5    6    7    8    9    10    11    12    
2    4    6    8    10    12    14    16    18    20    22    24    
3    6    9    12    15    18    21    24    27    30    33    36    
4    8    12    16    20    24    28    32    36    40    44    48    
5    10    15    20    25    30    35    40    45    50    55    60    
6    12    18    24    30    36    42    48    54    60    66    72    
7    14    21    28    35    42    49    56    63    70    77    84    
8    16    24    32    40    48    56    64    72    80    88    96    
9    18    27    36    45    54    63    72    81    90    99    108    
10    20    30    40    50    60    70    80    90    100    110    120    
11    22    33    44    55    66    77    88    99    110    121    132    
12    24    36    48    60    72    84    96    108    120    132    144
```

```java
public class MultidemsionalArray {

    public static void main(String[] args) {

        String[][] rowCol = new String[12][5];
        int[][] multTable = new int[12][12];
        int result;

        //fill the array with nested for-loops
        for (int row = 0; row < 12; row++){
            for (int col = 0; col < 5; col++){
                rowCol[row][col] = "row " + row + " col " + col;
            }
        }

        //print the array with nested for-loops
        for (int row = 0; row < 12; row++){
            for (int col = 0; col < 5; col++){
                System.out.printf("%s\t",rowCol[row][col]);
            }
            System.out.print("\r");

        }

        for (int i = 0;i <12; i++){
            for (int j = 0; j < 12; j++){
                //add one to our zero-based elements for 
                //the multiplication table
                result = (i+1)*(j+1);
                multTable[i][j] = result;
            }
        }

        for (int i = 0;i <12; i++){
            for (int j = 0; j < 12; j++){
                System.out.printf("%d\t",multTable[i][j]);
            }
            System.out.println("\r");
        }

    }
}
```

