# Development Workflow

- it will have acceptance tests for happy path scenarios
- acceptance tests will be in the `Acceptance` directory
- acceptance tests will use Testcontainers and Selenium
- acceptance tests will use DSL (ubiquitous language)
- in case of combinatorial complexity of acceptance tests, it will write application unit tests in `Unit/Application` directory
- in case of combinatorial complexity of acceptance tests, it will write domain unit tests in `Unit/Domain` directory
- every test will have given-when-then structure
- all testing infrastructure will be in the `Helpers` directory
- it will not use mocks, except for external services
- before test:
  - it will prepare the environment including the database if needed
  - it will seed the database with common data to be able to run the application
  - it will use entity factories using DSL (ubiquitous language) to create valid state before test