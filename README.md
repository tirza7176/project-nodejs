name:tirza simon;
email: t0527179413@gmail.com;

Running Locally (Local Server)
Ensure you have MongoDB installed and running on your machine.

Use the following MongoDB URI for the local database connection:
MONGO_URI_dev=mongodb://localhost/myrest_api_project
Create a .env file in the project root (if not already present) and add the above line along with other necessary environment variables.

Install dependencies:
npm install
Start the server:
npm run dev
The server will run on http://localhost:3000 (or the specified PORT).

Running on Cloud (MongoDB Atlas)
Use the following MongoDB URI for the cloud database connection:
MONGO_URI_PROD=mongodb+srv://t0527179413:ists8466@cluster0.lbcyzwb.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
Install dependencies:

npm install
Start the server:
npm run dev;
The server will run on http://localhost:3000 (or the specified PORT).

## Seeding the Database

To populate the database with initial data (users and cards), you can run the `seed.js` script. **Warning**: This script will delete all existing users and cards from the database and replace them with predefined data.

### How to run the seed script

Make sure your `.env` file is properly configured with the `MONGO_URI_DEV` variable.

Then, run:

node seed.js;



