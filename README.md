# Recipe
As a fun project working with databases and a lot of user input I wanted to create a plattform to share and find recipes from others, both individuals but also companies.
<br>
Feel free to download and test out for yourself, maybe you have fun ideas and new features to add. Feel free to contact me and maybe join the project!


# What you need:
  A database<br>
  A webserver/host capable of running/rendering PHP

# Set up database: (have server on preferred platform ready)

  1. Create database: (using SQL)
  ```SQL
  CREATE DATABASE recipe;
  ```

  2. Add the necessary tables withe the columns: <br>
    a. For the users:
      ```SQL
      CREATE TABLE adminUsers(
        id INT AUTO_INCREMENT PRIMARY KEY,
        uniqueID VARCHAR(32),
        dateJoined VARCHAR(64),
        userName VARCHAR(64),
        userEmail VARCHAR(320),
        firstName VARCHAR(64),
        lastName VARCHAR(64),
        primaryLanguage VARCHAR(64),
        otherLanguages VARCHAR(64),
        passWord VARCHAR(512),
        jobTitle VARCHAR(64),
        webSite VARCHAR(128),
        profileImage VARCHAR(256),
        recipesAdded INT
      );
      CREATE TABLE publicUsers(
        id INT AUTO_INCREMENT PRIMARY KEY,
        uniqueID VARCHAR(32),
        dateJoined VARCHAR(64),
        userName VARCHAR(64),
        userEmail VARCHAR(320),
        firstName VARCHAR(64),
        lastName VARCHAR(64),
        primaryLanguage VARCHAR(64),
        passWord VARCHAR(512),
        profileImageURL VARCHAR(256),
        recipesAdded INT
        );
      ```
      <br>
    b. For the content:
      ```SQL
      CREATE TABLE categories(
        id INT AUTO_INCREMENT PRIMARY KEY,
        uniqueID NVARCHAR(max),
        description VARCHAR(2500),
      );
      CREATE TABLE ingredients;
      CREATE TABLE recipes(
        id INT AUTO_INCREMENT PRIMARY KEY,
        uniqueID VARCHAR(32),
        description NVARCHAR(max),
        prepareTime INT,
        likeAmount INT,
        prepareTime INT,
        0ingredient-Unit VARCHAR(128),
        0ingredientAmount INT,
        1ingredient-Unit VARCHAR(128),
        1ingredientAmount INT,
        2ingredient-Unit VARCHAR(128),
        2ingredientAmount INT,
        3ingredient-Unit VARCHAR(128),
        3ingredientAmount INT,
        4ingredient-Unit VARCHAR(128),
        4ingredientAmount INT,
        5ingredient-Unit VARCHAR(128),
        5ingredientAmount INT,
        6ingredient-Unit VARCHAR(128),
        6ingredientAmount INT,
        7ingredient-Unit VARCHAR(128),
        7ingredientAmount INT,
        8ingredient-Unit VARCHAR(128),
        8ingredientAmount INT,
        9ingredient-Unit VARCHAR(128),
        9ingredientAmount INT,
        10ingredient-Unit VARCHAR(128),
        10ingredientAmount INT,
        11ingredient-Unit VARCHAR(128),
        11ingredientAmount INT,
        12ingredient-Unit VARCHAR(128),
        12ingredientAmount INT,
        13ingredient-Unit VARCHAR(128),
        13ingredientAmount INT,
        14ingredient-Unit VARCHAR(128),
        14ingredientAmount INT,
        15ingredient-Unit VARCHAR(128),
        15ingredientAmount INT,
        16ingredient-Unit VARCHAR(128),
        16ingredientAmount INT,
        17ingredient-Unit VARCHAR(128),
        17ingredientAmount INT,
        18ingredient-Unit VARCHAR(128),
        18ingredientAmount INT,
        19ingredient-Unit VARCHAR(128),
        19ingredientAmount INT,
      );
      ```
    
