### USER API - End Points

**Request Types**

- GET : to request data from the server
- POST : to submit data to be processed to the server

`/api/user/all - GET`: Returns list of all users.

`/api/user/create - POST`: Creating the user.

`/api/user/login - POST`: Takes care of logging in the user.

`/api/user/logout - POST`: Takes care of logging out the user.

`/api/user/<username>/exists - GET`: Check whether the particilar user exists or not.

`/api/user/ - GET`: Details about currently logged in user.

DONE

- Created venv using commands `python -m venv venv` and activate it through going to `venv/scripts`
- Installed flask, sqlalchemy, flask-sqlalchemy, flask-login, flask-migrate
- `Flask Migrate`: This module enables developers to quickly set up and starts the database schema migrations. Run commands `flask db init` to create migrations folder. Then run command `flask db migrate` and `flask db upgrade` to create database folder. And in this folder `user.db` should be created.
- To check if creation of user is succesful go to POSTMAN. Make POST request to `http://127.0.0.1:5000/api/user/create`. Go to Body, set it to form data. Add username and password fields. 