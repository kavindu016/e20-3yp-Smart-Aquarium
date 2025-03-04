# Backend
# First initialize the Project as follows

npm init -y
# Initializes a new Node.js project and creates a package.json file. The -y flag automatically answers "yes" to all prompts.

npm install express cors mysql2
# Installs the required dependencies.

express
# A web framework for Node.js to build the backend server.

cors
# Middleware to enable Cross-Origin Resource Sharing (CORS) for your API.

mysql2
# A MySQL client for Node.js to interact with the MySQL database.

npm install --save-dev nodemon
# Installs nodemon as a development dependency. It automatically restarts the server when file changes are detected.

npm install sequelize sequelize-cli
# Installs Sequelize (an ORM for Node.js) and its CLI tool for managing database migrations and models.

# Now we have these files
config/: Contains configuration files like database credentials.

migrations/: Stores migration files to create or modify database tables.

models/: Contains Sequelize models which are representations of database tables.

seeders/: Stores seed files to populate the database with initial data.

controllers/: Contains logic to handle requests and interact with models.

routes/: Defines API routes and links them to controllers.

app.js: Sets up the Express application and middleware.

server.js: Starts the server.

# next configure the database
update the config/config.json as needed for SQL

# app.js
Sets up the Express app.
Adds middleware (cors for enabling CORS and express.json for parsing JSON requests).
Defines a test route (/) to check if the server is running

# server.js
Starts the server on port 3001

# package.json
npm start: Runs the server in production mode.
npm run dev: Runs the server in development mode using nodemon which auto-restarts on file changes

# routes/userRoutes.js
Defines API routes
for example /api/users for getting all users and creating a new user.

# controllers/userController.js
Contains logic to handle requests
for example getAllUsers: Fetches all users from the database.

# app.js
Mounts the user routes under the /api prefix

# By now
Starts the server in development mode using nodemon.
The server will be accessible at http://localhost:3001


