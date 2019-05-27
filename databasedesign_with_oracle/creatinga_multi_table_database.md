# Creating A Multi\_Table Database

In the previous exercise we combined the authors and books in one table. This would work for a small database. But it's not appropriate for enterprise applications. It's more common to have a separate table for authors and a separate table for books. This makes your database more efficient, robust and easier to query. Let's see how we could make that work.

## Create the Books table

We can use every field from our previous table except the Author field. Create that table first.

* SKU \(stockkeeping unit - can contain numbers, dashes and possibly letters\)
* Book title \(text\)
* Description \(text\)
* Price \(double\)
* IsInStock \(true/false\)

## Create the Authors table

We would like to keep the author's first and last names separate so we can query by last name.

* FirstName \(text\)
* LastName \(text\)
* Address \(text\)
* City \(text\)
* State \(text\)
* ZIP \(text\)

## Bringing the Authors and Books together again

The following SQL statement will allow you to query the Author and Book table and bring the data back together again.

## Why did we make two tables?

It's possible some authors would write more than one book. When there was one book table then each book had the author listed with it. Stephen King has written 54 novels. The single-table database would store his name 54 times. Databases don't like to store redundant data. One of the key rules of databases is that each piece of data is in one place only. His name would belong in the Author table only. It's easier to store, update and query that way.

The database keeps track of the corresponding records with Primary Keys and Foreign Keys. The AuthorID is the primary key when it's in the Author table. It's the foreign key when it's in the Book table.

What happens if a book has two authors? We'll look at that next.

