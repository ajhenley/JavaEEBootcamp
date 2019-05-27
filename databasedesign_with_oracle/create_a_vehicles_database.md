# Create a vehicles database

Now it's your turn. Using all the new powers you've just learned, you will create a new database. This database will store information about people and their vehicles. 1. Create a table for people. You've already seen this so it should be simple. 2. Add at least five people to your people table. 3. Create a table for cars. 4. Populate the tables with some data. 5. Query the tables to show the people who own the cars.

## Next Steps

Did you decide to create a junction table? Why or why not?

What if you wanted to keep track of all the people who have owned a particular car? Create a table called PeopleCars. Include a field for PersonID, CarID and CurrentOwner. CurrentOwner field will be a Y/N field so it should be of type `char(1)`. Populate that field with Y for everybody. Next add records for an existing person as the owner of a car but not the current owner. Just like the authors. A car can have multiple owners. One person will be the current owner. Actually, your database _will_ allow more than one current owners but we're not creating a car co-op here. Just set one current owner for now.

