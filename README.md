# Movies Directory Table

## Introduction
- This is a challenge in Makers Module 3 - Databases
- I used this project to learn how to design and create a schema with a single table.
- `movies_directory_recipe.md` documents my design of the movies table
  
## Objectives
- [x] Design a single table schema from these user stories.
  - [x] As a person who loves movies,  
        So I can list all my favourite movies  
        I want to see a list of movies' titles.

  - [x] As a person who loves movies,  
        So I can list all my favourite movies  
        I want to see a list of movies' genres.

  - [x] As a person who loves movies,  
        So I can list all my favourite movies  
        I want to see a list of movies' release years.
- [x] Create the table by loading the SQL table file in psql.
- [x] To verify your work, make sure to run an INSERT query to insert a new movie record, and then a SELECT query to list the records.

## Setup
This project was made with postgreSQL database software. Here's how to install it:
```shell
# Install postgresql (use latest version)
$ brew install postgresql@15

# Make sure the installation directory is on your PATH environment variable
# Run this line from the Homebrew output
echo 'export PATH="/opt/homebrew/opt/postgresql@15/bin:$PATH"' >> ~/.zshrc

# Start a new terminal session
# Run this to start the postgresql software in the background.
$ brew services start postgresql@15

# You should get the following output:
==> Successfully started `postgresql@15` (label: homebrew.mxcl.postgresql@15)
```
Here's how to run this project:
```shell
# Clone the repository to your local machine
; git clone https://github.com/NatalieJClark/movies-directory-table.git YOUR_PROJECT_NAME

# Create the database
createdb movies_directory;

# Create the table by running the SQL table file with psql.
psql -h 127.0.0.1 movies_directory < movies_table.sql

# Navigate to the student_directory database with psql
psql -h 127.0.0.1 movies_directory

# View the created table with psql
SELECT * FROM movies;
