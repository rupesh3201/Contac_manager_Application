### Contact Manager Application
## Project Overview
Welcome to Contact Manager Application , your one-stop destination for Saving  and managing nuber cotact at same place . our platform is designed to provide comprehensive support, including detailed information with specific person.
![ Contact Manager Application]()
## Features
- Life Time Access
- Access it from anywhere
- Collections of Contact
- Fully Detailed Info
- Easy Registration
- 24*7 Support


## Table of Contents
Setup Instructions
API Documentation
User Registration
User Login
User Logout
CRUD Operations for Contacts
Technologies Used


Setup Instructions
Prerequisites
Node.js and npm should be installed on your system. You can download them from here.
A database such as MongoDB or any other of your choice (for production, we recommend using a cloud database).
1. Clone the repository
bash
Copy code
git clone https://github.com/your-username/contact-manager.git
cd contact-manager
2. Install Dependencies
Run the following command to install the required dependencies.

bash
Copy code
npm install
3. Set Up Environment Variables
Create a .env file in the root of the project and add the following variables:

makefile
Copy code
PORT=5000
DB_URI=mongodb://localhost:27017/contact_manager
JWT_SECRET=your_jwt_secret_key
PORT: The port number for your server to run.
DB_URI: The connection string to your database.
JWT_SECRET: A secret key used to sign JWT tokens for user authentication.
4. Run the Application
After setting up the environment variables, run the application:

bash
Copy code
npm start
The application should now be running at http://localhost:5000.

## db connection 
import mysql from 'mysql2/promise';
import dotenv from 'dotenv';


dotenv.config();


const db = mysql.createPool({
    host: process.env.DB_HOST,
    user: process.env.DB_USER,
    password: process.env.DB_PASSWORD,
    database: process.env.DB_NAME,
});

export default db;



## Technologies Used
Frontend : React js
Node.js: Backend JavaScript runtime.
Express: Web framework for Node.js to create RESTful APIs.
MongoDB: Database to store user and contact data.
JWT: JSON Web Token for user authentication.
Mongoose: MongoDB ODM to interact with the database.
