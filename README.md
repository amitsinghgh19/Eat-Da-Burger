# Eat-Da-Burger

**Creator**: `Amit Singh`

**Created on**: `June 20th 2019`

- - -

## ABOUT THE APP
A burger logging application with MySQL, Node, Express, Handlebars and an ORM. Node and MySQL are used to query and route data in the app, and Handlebars is used to generate HTML. The fully functional deploymed version of this app may be found at: https://evening-sierra-96535.herokuapp.com/

- - -
If you plan to test this app locally, please make sure you perform the following tasks:

1. While in the root directory of the app, run 'npm install' to install all the required npm packages
2. Run the schema.sql and seeds.sql files in the Database GUI of your choice.
3. Make sure your settings in the connection.js file in the 'config' directory match your specific local database.

- - -
Notes on MVC design pattern for this full-stack application:
------------------------------------------------------------

Model setup
-------------
Inside your burger directory, create a folder named models.

In models directory, you will find the burger.js file.
Inside burger.js, orm.js is imported into burger.js

Also inside burger.js, the code calls the ORM functions using burger specific input for the ORM.
Export at the end of the burger.js file.


Controller setup
------------------

In controllers directory, you will find the burgers_controller.js file.
Inside the burgers_controller.js file, the following are imported:

Express
burger.js

A router is created  for the app, and the router is exported  at the end of your file.



View setup
-----------
Inside the 'views' directory:
.
Create the index.handlebars file inside views directory.

Create the layouts directory inside views directory.


Create the main.handlebars file inside layouts directory.
Setup the main.handlebars file so it's able to be used by Handlebars.
Setup the index.handlebars to have the template that Handlebars can render onto.
Create a button in index.handlebars that will submit the user input into the database.
