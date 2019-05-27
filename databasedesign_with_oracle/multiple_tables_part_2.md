# Multiple Tables Part 2

In the last example we had two tables, authors and books. Each record in the book table contained a field for an authorID. This allowed you to find the corresponding author for that book. But there's a problem. If a book has two authors then where do you store the second author?

## The solution: bridge tables

Change the tables you have for Authors and Books and add a third table to keep track of just the corresponding IDs.

| **Author** |
| :--- |
| AuthorID |
| FirstName |
| LastName |

| **Book** |
| :--- |
| BookID |
| Title |
| Description |
| Price |

| **AuthorBook** |
| :--- |
| AuthorID |
| BookID |

Now you can store the same AuthorID with multiple BookIDs. What's more, you can store the same BookID with multiple AuthorIDs.

## Your Assignment

Create the AuthorBook table. To do that run the following code in SQL Developer. Then query the three tables. This is all shown in the SQL below. I've included some comments to help clarify things.

