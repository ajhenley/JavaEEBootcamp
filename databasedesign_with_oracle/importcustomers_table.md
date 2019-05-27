# Import Customers Table

This assignment has a lot of steps. But I'll walk you through them. And after that you will be an Oracle-SQL-Database Ninja.

Do you know what the most common database in business is? Think Excel. It seems every computer has a copy. It seems everybody uses it. Most people use it for the wrong stuff. Despite that it often works. In business, doing what works is more important than doing what's best.

In this exercise, you will be importing the data. Then you will follow a process that known as **Normalizing the Database**. There are a million ways to normalize your database. You're going to import a spreadsheet full of data. Then divide it into different tables. This is a realistic scenario. It plays out everyday throughout corporate America. Clients send you data. The data is a mess. You need that data in a database.

## Instructions for obtaining the customers.xlsx file

You can download the customers.xlsx file from the website.

## Here are the steps we will follow

1. Download the customers.xlsx file. It's an Excel file containing fake data about customers, addesses,companies and jobs.
2. Import the customers file into Oracle.
3. Write a query to find the number of unique companies in the table.
4. Create a new table for companies and move that data to the new table. Only move the unique companies. Then add a column to your customers table and update the the new column which is called CompanyID.
5. To set the value of your unique ID you can either create a sequence and a trigger or you can simply update that column to the row number as follows: `Update Company set CompanyId = rownum`.
6. Create a new table for cities and a new table for states. Move that data to the new tables in the same way you did above. Move unique cities and unique states to the two new tables. 
7. Delete those columns from this table and add keys to link to the new tables.
8. Create a query that recreates the list in Excel using joined tables.
9. Export the data as SQL import statements.

## Some help for you

To divide one table into multiple tables, you want to move all the unique company names to another table. Then delete them from the customer table. Here's the SQL that will accomplish that.

## Your assignment

Make another table for State and another table for City. Follow the same procedure to move that data to the new tables.

