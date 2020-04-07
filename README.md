# reverseEngineeringCode

config

- middleware/isAuthenticated.js
As a developer, we use this to make sure that the user is already authenticated.
- config.json
Contains login information to connect to different databases.
- passport.js
Utilizes the passport npm package in order to use user login authentication. Uses email and password to login and if there is no email/password in the database, it shows "incorrect email/incorrect password".

models

- index.js
We use this to collect the models and export them out using sequelize.

- user.js
Uses bcyrpt npm package for password and creates the user model.

public

- js/login.js
Uses jquery to make sure only the user with the correct email and password can get in, calls an axios request to verify.

- members.js
Makes a call to get ALL members.

- signup.js
Creates a new user.

- stylesheet/style.css
Use for custom styling other than styling libraries.

- login.html
Main page of the application, shows a login form, input for email and password, login button, and a link to sign up.

- members.html
Display page for users with a logout button.

- signup.html
Signup page for new user, input for email and password and a link to sign up.

routes

- api-routes.js
Uses api calls to post login/signup, get logout and user data

- html-routes.js
Contains the routes to send users to the members page.

- package.json
Contains the npm packages used.

- server.js
Contains npm packages used, sets up ports and connects routes, sets up middleware and where our application is abe to work with the json data.

