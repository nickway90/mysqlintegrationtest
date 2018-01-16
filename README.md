# mysqlintegrationtest

This package provides functionality for running parallel database integration test with MySQL.

## How it works

It needs a connection to mysql and will use that connection to create some databases that will be used by each of the test function. In other words, each test function will have their own database. `CreateTestDatabase` will return cleanup function for dropping the test-database.
