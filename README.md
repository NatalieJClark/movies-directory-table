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

```shell
# Clone the repository to your local machine
; git clone https://github.com/NatalieJClark/movies-directory-table.git YOUR_PROJECT_NAME

# Create the database
createdb movies_directory;

# Create the table by running the SQL table file with psql.
psql -h 127.0.0.1 movies_directory < movies_table.sql

# Enter psql
psql

# Connect to the student_directory database
\c movies_directory

# View the created table
SELECT * FROM movies
