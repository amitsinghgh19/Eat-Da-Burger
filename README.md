# Eat-Da-Burger

**Creator**: `Amit Singh`

**Created on**: `June 20th 2019`

- - -

## ABOUT THE APP
A burger logging application with MySQL, Node, Express, Handlebars and an ORM. Node and MySQL are used to query and route data in the app, and Handlebars is used to generate HTML. 

See screen-shot below:
    ![Results](/public/assets/img/deployedApp.png)
- - -

## Demo Link
The fully functional deployed version of this app may be found here.
* [Link to the web site hosted on Heroku](https://evening-sierra-96535.herokuapp.com/)

## GitHub Link  
* [Link to my repository](https://github.com/amitsinghgh19/Eat-Da-Burger.git)

- - -

## App Functionality

*A fun app that lets a user input the name of a burger they want to eat.

*Once submitted, the burger is displayed in text on the left side of the page where it's waiting to be devoured.

*Each burger in the waiting area also has a Devour it! button. Once clicked, the burger will move to the right side of the page.

*Every burger entered is stored in the database.

- - -

## Below is a summary of how the app is structured and operates

- config
    - connection.js
        - establish database connection
    - orm.js
        - object for all of our SQL statement functions
            - all selects all burgers from database
            - create creates a new burger and inserts it into the database
            - update updates a database change
            - delete removes burger from database

- controllers
    - burger_controllers.js
        - routing for our burger app
            - get pulls all burgers from database and displays on screen
            - post and create will post new burger on screen and in database      
            - put and update will update database and move burger to devoured after button click
            - delete will remove burger from screen and database

    - db
        - schema.sql
        - seeds.sql
      
- models
    - burger.js
        - importing orm.js to create functions that will interact with database
    
    - public
        - assets for images, css and simple js file
        - app.get to pull survey page

- views
    - handlebars functionality

- server.js
    - configuration of server and application

- - -
## Installation
To run the application locally, first clone this repository with the following command.

#### App Setup



1. Create a GitHub repo called `burger` and clone it to your computer.
	git clone https://github.com/amitsinghgh19/Eat-Da-Burger.git



2. Make a package.json file by running `npm init` from the command line.


## Next, install the application dependencies.


3. Install the Express npm package: `npm install express`.



4. Create a server.js file.



5. Install the Handlebars npm package: `npm install express-handlebars`.



6. Install the body-parser npm package: `npm install body-parser`.



7. Install MySQL npm package: `npm install mysql`.



8. Require the following npm packages inside of the server.js file:
   
* express
   * body-parser

9. Make sure to create a MySql database using schema.sql.

Finally, run the node server.js locally.

Now, open the application at the URL: http://localhost:8080/.


-----------------------
##Technologies Used
* HTML
* CSS
* JavaScript
* Node.js
* MySQL
* JawsDB
* ORM
* Heroku

##Frameworks and Packages
* Express.js
* jQuery
* Handlebars
* Body-Parser
* Method-override


#### Background Picture Reference
- https://wallpapersite.com/
- https://www.google.com/