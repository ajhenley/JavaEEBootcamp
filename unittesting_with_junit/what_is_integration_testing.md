# What is integration testing?

Unit tests allow you to validate your application's business logic. Unit tests do not ensure the deployability of your amazing shiny new Java application.For that we turn to integration testing.

## Integration Testing

* Example: getting data out of the database and sending an email to the logged in user
* verifies implementation of individual components and their interconnected behavior
* tests the system using real data
* depends on the environment
* Failed integration tests do not mean you have a coding error. Tests could fail even if your code is correct. Some reasons might include:
  * incorrect configuration information for database or mail server
  * network problems

## Unit Testing

* Example: testing that your method to calculate a person's age will returns the correct result
* only tests your Java code
  * generally tests one method at a time
  * uses mocked data
* Failed unit tests indicates the code has changed

