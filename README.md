# Sequelize-Inspector

Inspect the given code and analyze how it works. Write a tutorial explaning every file and its purpose in as fine as detail as possible. If one file is dependent on other files, be sure to let the user know. The app allows users to sign up and log into the app with an email and encrypted password, and logout.


## Installed With

- npm install
- mysql database called passport-demo


## Tech Used

- express
- express-session
- passport
- passport-local
- mysql
- sequelize
- bcryptjs
- JSON
- Javascript
- HTML
- CSS


## Files and Folders Explained

## server.js

The server.js file requires express, express-session, and a route from the passport.js. It sets up the PORT and creates the express variable and how to use it. If creates the routes to both the api-routes.js and html-routes.js files. If also sets up the connection with of the PORT with sequelize.

## html-routes.js

This file redirects to the different html files depending on what the user chooses. It requires the path and routes to the isAuthenticated.js file for authentication. Each app.get function routes to the html file they correspond to. 

## login.html, members.html, signup.html

Each html file displays to the user the login, sign up, or members page based on the route chosen. They pull from the login.js, signup.js, and signup.js files.

## login.js, members.js, and signup.js 

These files hook from the html pages to update the email and password on the signup page, or login on the login page. 

## api-routes.js 

Pulls db data from models folder and requires passport for authentication. The get function is how the client side js files work with this file. The post functions authenticate and create the login/signup routes to send the data to the models folder.

## user.js

For creating username and passord. Middleware for encryption and security for the database. 

## index.js

Adds fs, path, sequelize, and the sequelize template. Connects and creates tables in the database through sequelize. Pulls the config.json data 

## passport.js

Acts like the toll booth to check for authentication. Passport template with functionality for passport-local. 

## isAuthenticated.js

Checks password to restrict routes for users. 








## Author 

### Ry Hull

#### GitHub Repo
 - https://github.com/ryandelonhull
#### Linked In
 - https://linkedin.com/in/ryan-hull-94003144
#### Portfolio
 - https://ryandelonhull.github.io/Bootstrap-Portfolio/



  ## *Acknowledgments*

 Big thank you to Roger, Kerwin, Manuel and my tutor for wading into the deep waters of coding with the class and keeping me afloat with their instruction and guidance. Thank you to my fellow classmates for including me in the study and homework sessions as working together on a problem has been a great teacher also.
