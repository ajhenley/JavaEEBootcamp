# More SQL Commands

It's time to explore SQL further. I'll give you several SQL statements which you can explore by runing against your newly created Customers table. You will need to type the SQL statements into SQL Developer and click the run icon to execute them. Each statement should end with semi-colon to separate it from the next statement you enter.

Your customer database consists of multiple tables. You should have the following tables: Customers, States, Cities and Companies. Each table contains an ID field which is its primary key. You should also have bridge tables to link the customers with their companies

Select the name of all our customers from one table Filter the names to only show those named Smith using = Filter the names to only show those named Smith using LIKE

Select the name and address of all the Smiths from multiple tables Select the name and address, city, state, and zip for everyone and this time use table aliases and order by last name then order by state, city, last name

Update a particular person who has become a Smith Change someone's address Add a new ZIP and update selected customers to live in the new ZIP based on street name and old ZIP ID. Make sure this finds multiple rows.

Delete a customer, delete a company

begin a tranaction, delete a customer and company then rollback then query to see the changes run select to show there aren't any updated records begin trans, change a customer and company and commit then query to see changes run select to show updated records

use subqueries to select all the people at one company

create left outer join, right outer join, full outer join, self join select all the people who are not working select all the people who don't work for a particualr company

compound where clauses select all the people who are a particular position in a particular state

grouping/having - select counts by state, counts by company order the results by state, company order the results by company then state

