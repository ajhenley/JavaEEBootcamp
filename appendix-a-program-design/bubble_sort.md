# Bubble Sort

The Bubble Sort algorithm considers each element in the list. When the algorithm finds two consecutive elements out of order, they get swapped. The result is a sorted list. The largest element "sinks" to the bottom and the smaller elements "float" to the top.

The algorithm traverses the unsorted part of the array repeatedly. Consecutive elements are compared during each traversal. When they are out of order, they are swapped using temporary variable.

The bubble sort will continue until the list is sorted. After the first pass, the largest item will occupy the last position but the other items may not be fully sorted. Multiple passes \(represented by i\) will occur until the list is sorted. At that time the conditional statement on line 3 will evaluate to false causing execution to fall the end of the algorithm.

Note that **a** is the list, **n** represents the number of elements in the list and **temp** represents the temporary \(swap\) variable.

```text
    For i = 0 to n - 1
        For j = 1 to n - 1
            If (a(j) > a(j + 1))
                temp = a(j)
                a(j) = a(j + 1)
                a(j + 1) = temp
            End-If
        End-For
    End-For
```

Test the bubble sort algorithm by having it sort the letters in your name.

Next sort the following numbers: 34,29,69,33,88.

If you're still not convinced then sort the Presidents \(since Kennedy\) by last name: Kennedy Johnson Nixon Ford Carter Reagan Bush Clinton Bush Obama

Test the algorithm on an the following list: 1,2,3,4,5. What happens?

How would you change the algorithm to sort in descending order?

