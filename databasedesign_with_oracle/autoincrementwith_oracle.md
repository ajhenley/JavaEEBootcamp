# Autoincrement with Oracle

## Oracle doesn't include an autoincrement type...

Here's an example how to add a sequence in Oracle 11g. If you're working with Oracle 12c the process has been simplified though this will work as well.

## Create a table

## You will need to create a sequence

## And create a trigger for the sequence

## Then run:

Alternatively, you can create an identity column from the Edit Table dialog in SQL Developer. Select the Identity tab. Then select the trigger name and column.

Remember, if you create a sequence and then delete the table the sequence continues to exist. If you recreate the table you won't be able to recreate the sequence. If you use the existing sequence then the numbering will pick up where the old sequence left off.

