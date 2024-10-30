# Connecting-python-with-Oracle
To write a python program to get data using faker and upload into Oracle database

Summary of the Program
Install Necessary Libraries:

Use the Faker library to generate synthetic data and cx_Oracle to connect to and interact with the Oracle database.

1..pip install Faker cx_Oracle


2..pip install faker

Set Up Database Connection:

Establish a connection to the Oracle database using cx_Oracle.connect(). Provide your Oracle database credentials (username, password, and database URL).

Create a Table :

Use SQL commands within Python to create a table in the Oracle database to store the generated data 
(e.g., a table called employees with columns for id, name, and salary).


Generate Fake Data:

Use the Faker library to generate random names and salaries. For example, fake.name() generates a random name, and round(random.uniform(30000, 100000), 2) can generate a random salary between 30,000 and 100,000.

Define a function that creates multiple records with Faker data.

Insert Data into Oracle Database:

Use cursor.execute() to insert each generated record into the database.

Use connection.commit() to ensure data is saved to the database.

Close Connection

