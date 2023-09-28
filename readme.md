
# Backend Phase README

## Project Overview

This is the backend phase of our project, responsible for handling server-side logic and data management. Below, you'll find important information about the project's structure, technologies used, and how to work with it.

## Project Structure

The backend project is organized as follows:

- **config/**: Contains configuration files for the backend, including settings for database connections, authentication, and email sending using Nodemailer.

- **controllers/**: Controllers handle the application's business logic, including user, order, and product-related operations.

- **data/**: This directory may contain seed data or scripts used to initialize the database with initial data.

- **middleware/**: Middleware functions, including JWT validation, that are used to intercept and process incoming requests before they reach the route handlers.

- **models/**: Defines the data models for the application, including models for users, orders, and products.

- **routes/**: Contains route files that define the API endpoints and their associated controllers. There are separate route files for users, orders, products, and potentially file uploads.

- **utils/**: Utility functions and helper modules used across different parts of the application. This  include JWT-related utilities.

- **.env**: Configuration file for environment variables, including the MongoDB URI, JWT secret, and PayPal client ID.

## Technologies Used

The backend phase utilizes the following technologies:

- **Node.js**: The JavaScript runtime used for building server-side applications.

- **Express.js**: A web application framework for Node.js, used for routing, middleware, and handling HTTP requests.

- **MongoDB**: A NoSQL database for data storage, often used for its flexibility and scalability.

- **JSON Web Tokens (JWT)**: Used for authentication and securing API endpoints.

- **Nodemailer**: For sending emails 

## Dependencies

- **bcrypt**: Used for hashing and salting passwords, enhancing security for user authentication.

- **body-parser**: Middleware for parsing JSON and URL-encoded request bodies, making it easier to handle incoming data.

- **cors**: Enables Cross-Origin Resource Sharing (CORS) to handle requests from different origins, allowing your frontend to communicate with the backend.

- **dotenv**: A module for loading environment variables from a `.env` file, keeping sensitive information like database credentials and API keys secure.

- **express**: The core web application framework for Node.js, simplifying routing, middleware, and HTTP request handling.

- **express-async-handler**: A utility for handling asynchronous errors in Express route handlers, ensuring better error handling.

- **jsonwebtoken**: Used for generating and verifying JSON Web Tokens (JWTs) for user authentication and authorization.

- **mongoose**: An Object Data Modeling (ODM) library for MongoDB, simplifying database interactions and schema management.

- **morgan**: Middleware for logging HTTP requests, which can be useful for debugging and monitoring.

- **multer**: Middleware for handling file uploads, if your application involves file uploading functionality.

- **nodemailer**: A module for sending emails, potentially for user notifications, password reset functionality, or other email-based features.

- **nodemon**: A development tool that automatically restarts the Node.js server when changes are detected, making the development process smoother.




## Getting Started

To get started with the backend phase, follow these steps:

1. Install the required dependencies:
   ```bash
   npm install
   ```

2. Configure your environment variables in the `.env` file, including the MongoDB URI, JWT secret, and PayPal client ID.


3. Configure your mailer on config/mailer.js


4. Start the backend server:
   ```bash
   npm start
   ```

