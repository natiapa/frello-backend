# Frello Backend - Project Management Application

The backend of the Frello project management application is a robust and production-ready server built with Node.js and Express. It handles API requests, user authentication, data storage, and real-time updates using Socket.IO. The backend is designed to support the dynamic and collaborative nature of the project, allowing multiple users to interact and manage tasks efficiently.

## Features

- **User Authentication:** Uses passport.js for user authentication, including Google OAuth 2.0.
- **Real-time Collaboration:** Utilizes Socket.IO for real-time updates to support collaborative task management.
- **Data Management:** Manages boards, lists, and tasks, providing a comprehensive API for the frontend to interact with.
- **Secure:** Implements bcrypt for password encryption and cryptr for secure data management.
- **Session Management:** Utilizes express-session and connect-mongo for session storage and management.
- **Cross-Origin Resource Sharing (CORS):** Enabled to allow frontend-backend communication.

## Technologies Used

- **Node.js** - Runtime environment for building server-side applications.
- **Express** - Web framework for building the RESTful API.
- **MongoDB** - NoSQL database for storing project, board, and task data.
- **Socket.IO** - For real-time, bidirectional communication between the server and clients.
- **Passport** - For user authentication, including Google OAuth 2.0.
- **bcrypt** - For secure password hashing.
- **dotenv** - To manage environment variables.
- **Nodemon** - For hot-reloading during development.

## Getting Started

### Prerequisites

- Node.js and npm installed on your machine.
- A running instance of MongoDB.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/natiapa/frello.git
    ```
2. Navigate to the backend directory:
    ```bash
    cd frello-backend
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```
4. Create a `.env` file in the root directory to store your environment variables (e.g., MongoDB URI, session secrets).
5. Start the development server:
    ```bash
    npm start
    ```

### Scripts

- **`npm run start`** - Starts the server using Nodemon for development.
- **`npm run dev`** - Starts the server in development mode.
- **`npm run server:prod`** - Runs the server in production mode (Windows).
- **`npm run server:prod:mac`** - Runs the server in production mode (Mac/Linux).

## Folder Structure

- `server.js` - The main entry point of the backend server.
- `routes/` - Contains all route files for API endpoints.
- `controllers/` - Includes the logic for handling requests and interacting with the database.
- `models/` - Defines the database schema for MongoDB.
- `middlewares/` - Includes middleware functions for authentication and other tasks.
- `services/` - Handles communication with external services and utilities.

## Credits

This project was developed collaboratively by:
- [Yana Pletner](https://github.com/YanaPletner)
- [Avi Friedman](https://github.com/avi-friedman-IL)
- [Nati Apa](https://github.com/natiapa)
- Or Cohen

## Dependencies

- **bcrypt** - For password hashing.
- **connect-mongo** - To store session information in MongoDB.
- **cookie-parser** - For parsing cookies in the request headers.
- **cors** - For handling Cross-Origin Resource Sharing (CORS).
- **cryptr** - For secure data encryption.
- **dotenv** - To manage environment variables.
- **express** - Web framework for building the API.
- **express-session** - For session management.
- **mongodb** - MongoDB client for interacting with the database.
- **passport** - Authentication middleware for Node.js.
- **passport-google-oauth20** - For Google OAuth 2.0 authentication.
- **socket.io** - For real-time communication between server and client.

## Dev Dependencies

- **nodemon** - For hot-reloading during development.

