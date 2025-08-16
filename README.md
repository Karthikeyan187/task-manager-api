# Task Manager API

## Introduction
Welcome to the Task Manager API, a robust and scalable RESTful web service designed to help users manage their tasks efficiently. Built with Express.js and MongoDB, this API provides a seamless experience for task management, ensuring secure user authentication and data integrity.

## Key Features
- **User Authentication**: 
  - Secure signup and login endpoints utilizing JSON Web Tokens (JWT) for protected routes.
  
- **Task Management**:
  - Create, read, update, and delete tasks with ease.
  - Each task can have a title, description, and completion status.

- **Validation**:
  - Comprehensive validation for user inputs to ensure data integrity and provide meaningful error messages.

- **Health Check Endpoint**: 
  - A dedicated endpoint to monitor the API's operational status.

## Technical Stack
- **Backend Framework**: Node.js with Express.js
- **Database**: MongoDB, managed with Mongoose
- **Authentication**: JSON Web Tokens (JWT) for secure access
- **Validation**: Input validation using express-validator
- **Environment Management**: dotenv for managing sensitive configuration values
- **Security**: Helmet for securing HTTP headers, CORS for cross-origin resource sharing

## Getting Started
To get started with the Task Manager API, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/task-manager-api.git
   cd task-manager-api
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```

3. **Set Up Environment Variables**:
   Create a `.env` file in the root directory and add the following:
   ```
   PORT=3000
   MONGODB_URI=your_mongodb_uri
   JWT_SECRET=your-secret-key
   NODE_ENV=development
   ```

4. **Start the Server**:
   ```bash
   npm run dev
   ```

## API Endpoints
- **Authentication**:
  - `POST /api/auth/signup`: Register a new user.
  - `POST /api/auth/login`: Authenticate user and retrieve a token.

- **Task Management**:
  - `POST /api/tasks`: Create a new task.
  - `GET /api/tasks`: Retrieve all tasks for the logged-in user.
  - `PUT /api/tasks/:id`: Update a specific task by ID.
  - `DELETE /api/tasks/:id`: Delete a specific task by ID.

- **Health Check**:
  - `GET /api/health`: Check the API status.

## Contributing
Contributions are welcome! If you have suggestions for improvements or find bugs, please open an issue or submit a pull request.

## Acknowledgments
- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)
- [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)
- [bcrypt](https://www.npmjs.com/package/bcrypt)
