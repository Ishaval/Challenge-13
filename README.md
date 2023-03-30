# E-Commerce Back End

## Description

This project provides the back-end implementation for an e-commerce site. The main goal is to build a working Express.js API that uses Sequelize to interact with a MySQL database.

## Table of Contents

*[USER STORY](#user-story)

*[ACCEPTANCE CRITERIA](#acceptance-criteria)

*[INSTALLATION AND SETUP](#installation-and-setup)

*[DATABASE MODELS](#database-models)

*[MODEL ASSOCIATIONS](#model-associations)

*[API ROUTES](#api-routes)

*[SEEDING THE DATABASE](#seeding-the-database)

*[WALKTHROUGH VIDEO](#walkthrough-video)

*[GRADING REQUIREMENTS](#grading-requirements)

*[LICENSE](#license)


## User Story

```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

```

## Acceptance Criteria

```md
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database
```

## Installation and Setup
```md
1. Clone the repository.

2. Run `npm install` to install the required packages.

3. Create a `.env` file in the root folder and add your MySQL username, password, and database name.

4. Run the schema.sql file in the db folder to create your database with MySQL shell commands.

5. Run `npm run seed` to seed data to your database for testing.

6. Run `npm start` to start the server.
```

## Database Models
```md
The database contains four models:

1. Category
2. Product
3. Tag
4. ProductTag

```

## Model Associations

```md
The following associations are created between the models:

1. Product belongs to Category, and Category has many Product models.

2. Product belongs to many Tag models, and Tag belongs to many Product models, using the ProductTag through model.
```


## API Routes

```md
The application contains API routes for the following actions:

1. GET routes to return all categories, products, and tags.
2. GET routes to return a single category, product, and tag by ID.
3. POST routes to create new categories, products, and tags.
4. PUT routes to update categories, products, and tags by ID.
5. DELETE routes to delete categories, products, and tags by ID.
```


## Seed the Database

Run npm run seed to seed data to your database for testing.

## Walkthrough Video

[video](./video/2023-03-30%2013-57-23.mkv)



