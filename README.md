# Techstack

- **sqlc** : used in Go for generating type-safe APIs from SQL queries. It allows developers to write SQL queries in .sql files and then automatically generates Go code that provides type-safe access to the database.

- **makefile**: a script containing a set of commands used to automate tasks, typically for compiling and building software projects. It specifies dependencies and rules for executing commands efficiently.

- **Go migration** : used to manage database schema changes in Go applications. They automate the process of creating, applying, and reverting database migrations, ensuring consistency and reproducibility across different environments.

- **lib/pq** : `lib/pq` is a Go driver for PostgreSQL databases. It enables Go programs to interact with PostgreSQL databases by providing an interface to execute SQL queries, insert, update, delete data, and more.

- **testify** : Go code (golang) set of packages that provide many tools for testifying that your code will behave as you intend.

# Steps

1. Installing docker, sqlc, database manager(like DataGrip, TablePlus, etc), make, Go migration

2. Configure WSL2 + Go + VSCode + Docker + Make + Sqlc

3. new "make" commands can be created throughout the process

4. Installing and using Docker. Creating a PostgreSQL container and connecting to it using a database manager(like DataGrip, TablePlus, etc)

5. Run and write a Database Migration using Go Migrate. This helps in defining database schemas.

6. Generate CRUD GoLang code using SQLC.

    - Install SQLC and initialize it using `sqlc init`

    - From https://github.com/sqlc-dev/sqlc/tree/v1.4.0 copy the settings configuration available in the "Settings" section and then modfiy it according to your need.

    - Create the directories and modify them in the "sqlc.yaml" accordingly.

    - Add the sql queries you need accordingly throughout the process and generate Go code by ```make generate```(install make to run this command).

7. Create GoLang unit tests for databse CRUD with random data

    - Install `lib/pq` and `tetsify` from using their respective go commands.

    - Create a go test file for all the relations.
