# Searching and Printing an Array

* A linear search of an array looks at each element starting with first

  ```text
  Linear_search_of_an_array
   Set max_num_elements to required value
   Set element_found to false
   Set index to 1

   DOWHILE(NOT element_found)AND(index &lt;= max_num_elements)
        IF array(index)= input_value THEN
          Set element_found to true
        ELSE
          index = index + 1
        ENDIF
   ENDDO

   IF element_found THEN
       Print array (index)
   ELSE
       Print &lsquo;value not found&rsquo;, input_value
   ENDIF
  END
  ```

## Binary search of an array

* faster than linear search for arrays with &gt; 25 elements
* first, sort elements into ascending sequence
* next, locate the middle element
* then determine if your element is in the first half or second
* repeat the process with the selected half of the array

\`\` Binary\_search\_of\_an\_array

Set element\_found to false Set low\_element to 1 Set high\_element to max\_num\_elements

DOWHILE \(NOT element\_found\) AND\(low\_element &lt;= high\_element\) index = \(low\_element + high\_element\)/2

```text
   IF input_value = array (index)THEN
      Set element_found to true
   ELSE
      IF input_value &lt; array (index)THEN
          high_element = index &ndash; 1
      ELSE
          low_element = index + 1
      ENDIF
   ENDIF
```

ENDDO

IF element\_found THEN Print array \(index\) ELSE Print ‘value not found’, input\_value ENDIF END

```text
####Writing out contents of an array
* use DO loop
* start with first element
* write each element until done
```

Write\_values\_of\_array DO index = 1 to number\_of\_elements Print array\(index\) ENDDO END

\`\`\`

