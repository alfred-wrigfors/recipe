# Recipe

# What you need:
  A database<br>
  A webserver/host capable of running/rendering PHP

# Set up database: (have server on preferred platform ready)

  1. Create database: (using SQL)
  ```SQL
  CREATE DATABASE recipe;
  ```

  2. Add the necessary tables: <br>
    a. For the users:
      ```SQL
      CREATE TABLE adminUsers;
      CREATE TABLE publicUsers;
      ```
      b. For the content: <br>
      ```SQL
      CREATE TABLE categories;
      CREATE TABLE ingredients;
      CREATE TABLE recipes
      ```
