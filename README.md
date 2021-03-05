# E-commerce Back End application

## Purpose of application
Internet retail, also known as e-commerce, is the largest sector of the electronics industry, having generated an estimated US$29 trillion in 2017 (Source: United Nations Conference on Trade and Development). E-commerce platforms like Shopify and WooCommerce provide a suite of services to businesses of all sizes. Due to the prevalence of these platforms, developers should understand the fundamental architecture of e-commerce sites. This application builds the back end for an e-commerce site.

## Description
This application uses Express.js API and configure it to use Sequelize to interact with a MySQL database.Db name, user name and password are saved in .env file using which user can connect to database using sequelize.
* run command "source db/schema.sql" from mysql terminal to create database schema.
* run command "npm install" from gitbash ti install all dependencies in package.json file. 
* application dependecies:
 "dependencies": {
    "dotenv": "^8.2.0",
    "express": "^4.17.1",
    "mysql2": "^2.1.0",
    "sequelize": "^5.21.7"
  }
* run command "npm run seed" to seed tables with data.
* run command "npm start" or "node server.js" from gitbash terminal to start application.
* Category API route:
    1. get - api/categories - to get all categories
    2. get - api/categories/id -  to get category of specific id
    3. Post - api/categories - Create new category
    4. Put - api/categories/id - to update category
    5. Delete - api/categories/id - to delete category
* Product API routes:
    1. get - api/products - to get all products
    2. get - api/products/id -  to get product of specific id
    3. Post - api/products - Create new product
    4. Put - api/products/id - to update product
    5. Delete - api/products/id - to delete product
* Tag API routes:
    1. get - api/tags - to get all tags
    2. get - api/tags/id -  to get tag of specific id
    3. Post - api/tags - Create new tag
    4. Put - api/tags/id - to update tag
    5. Delete - api/tags/id - to delete tag

## User story
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

## Acceptance crieteria
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database

## Mock-Up
The following animations show examples of the application's API routes being tested in Insomnia Core.

<div>
    <img src="./images/get.gif" width="400px"/> 
</div>

<div>
    <img src="./images/getid.gif" width="400px"/> 
</div>

<div>
    <img src="./images/crud.gif" width="400px"/> 
</div>

## Built With
* node js
* mysql database
* express js 
* dotenv
* sequelize

