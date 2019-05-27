# Debugging Activity: Print Timesheet Records

Chanchal is the project manager for a small software development project. Each week she wants a report of the employees who have worked on her project, separated by full-time and part-time.

She has developed the pseudocode below but since she is the project manager and not the programmer it has an error in it. It's your job to fix the error to make her look good to the team. She plans to present the report at the standing meeting tomorrow morning. If you succeed she will look good and remember you when assigning new tasks.

You had told her that she would need a DOWHILE loop to control the repetition And an IF statement to select ‘FT’ records

## Incorrect Results - find and fix the error

```text
Print_Hours_Billed_To_Project
Print "Employee Hours Billed to Project" heading
    Read timesheet record
    DOWHILE morerecords exist
        IF timesheet_status = &lsquo;FT&rsquo; THEN
            Print EmployeeID, Department, Billing Rate, Hours Worked
        ENDIF
    ENDDO
    Read timesheet record
END
```

```text
Employee Hours Billed to Project
Full-Time employees
    10335 Finance    Smithers  $110.00/hour 24 hours
    21555 Marketing  Wiggims   $75.00/hour  10 hours
    31004 IT         Burns     $150.00/hour 20 hours
```

