# Different types of testing

**Unit tests** - used to check that your classes and methods function as expected. The more tests you run the more certain your code works as you've intended. Unit tests are easy to create and even easier to run so you can check your application frequently. External objects such as a database can be simulated. Use mock objects to make your tests independent of the larger system and easy to run.

**Customer's tests** are functional, system, and acceptance tests. They check the behavior of the system as a whole as expected by the customer.

**Integration tests** combine customer tests and unit tests. Integration tests concern themselves with the interaction of your application's parts. You're no longer creating mock objects. You are testing the actual database, network, email and file systems.Integration testing takes more time and coordination. You may even need to load test data into your database or application. Integration tests may also use special external libraries.

