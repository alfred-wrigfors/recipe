# SQL.md
This is an instruction on getting the database with tables ready.


# Set up database: (have server on preferred platform ready)

  1. Create database: (using SQL)
  ```SQL
  CREATE DATABASE recipe;
  ```

  2. Add the necessary tables with the the columns: <br>
    1. For the users:
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
      
  2. Add the necessary tables with the the columns: <br>
    1. For the content: <br>
      1. For the different categories:
        ```SQL
        CREATE TABLE categories(
          id INT AUTO_INCREMENT PRIMARY KEY,
          uniqueID NVARCHAR(max),
          description VARCHAR(2500),
        );
        ```
        
      2. For the different ingredients
        ```SQL
        CREATE TABLE ingredients(
          id INT AUTO_INCREMENT PRIMARY KEY,
          uniqueID VARCHAR(32),
          name VARCHAR(64)
          description NVARCHAR(max),
        );
        ```
        
      3. For the recipes them selfs:
        ```SQL
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
    
