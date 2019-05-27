# Change Activity: Process Timesheet Records

In true project manager fashion Chanchal has asked you to also print the part-time employees. But they should be separate from the full-time employees. The report she wants looks like this:

```text
Employee Hours Billed to Project
Full-Time employees
    10335 Finance    Smithers  $110.00/hour 24 hours
    21555 Marketing  Wiggims   $75.00/hour  10 hours
    31004 IT         Burns     $150.00/hour 20 hours
Part-Time employees
   20045 Finance     Flanders  $25.00/hour  10 hours
```

## Incorrect Results - find and fix the error

```text
Print_Hours_Billed_To_Project
Print "Employee Hours Billed to Project" heading
    Read timesheet record
    DOWHILE morerecords exist
        IF timesheet_status = "FT" THEN
            Print EmployeeID, Department, Billing Rate, Hours Worked
        ENDIF
    ENDDO
    Read timesheet record
END
```

Alter the previous activity to print the report as shown above.

