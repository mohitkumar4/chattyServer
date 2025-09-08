ChattyServer - Full-Stack Real-Time Chat Application


A full-stack, real-time messaging application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) and powered by Socket.IO for instant, bi-directional communication. This platform allows users to sign up, log in, find other users, and engage in private, one-on-one conversations with live online presence indicators and image sharing capabilities.

✨ [Live Site / Deployed App Link]
Features
This project is a complete full-stack application with a feature-rich client and a robust backend.

Backend Features
Real-Time Communication: Implemented with Socket.IO for instant message delivery and live online user status tracking.

Secure RESTful API: Built with Node.js and Express.js, featuring protected endpoints for all sensitive operations.

JWT Authentication: Secure user authentication and session management using JSON Web Tokens stored in httpOnly cookies to prevent XSS and CSRF attacks.

Database Management: Utilizes MongoDB with Mongoose for efficient data modeling and retrieval of users, messages, and conversations.

Cloud Media Storage: Integrates with Cloudinary for scalable cloud-based storage of user profile pictures and shared images.

Environment-Based Configuration: Uses .env files for secure management of sensitive credentials and application settings.

Frontend Features
Component-Based UI: Developed with React.js for a modular, reusable, and maintainable codebase.

Centralized State Management: Employs Zustand for efficient and predictable global state management of user authentication, messages, and online users.

Responsive Design: Styled with Tailwind CSS for a modern, mobile-first, and fully responsive user interface that works on any device.

Client-Side Routing: Uses React Router to handle navigation and create a seamless single-page application (SPA) experience.

Real-Time Updates: The UI listens for WebSocket events to update messages and user presence indicators instantly without needing to refresh the page.

User Experience (UX) Enhancements: Includes features like skeleton loading screens, toast notifications for feedback, and image previews before uploading.

Tech Stack
The project is built using a modern and powerful technology stack:

Category	Technology
Frontend	React.js, Zustand, React Router, Tailwind CSS, Axios, Socket.IO Client
Backend	Node.js, Express.js, MongoDB, Socket.IO
Database	MongoDB (with Mongoose)
Authentication	JSON Web Tokens (JWT), bcrypt.js (for password hashing)
Media Storage	Cloudinary API
Deployment	Render (or any similar PaaS)
Dev Tools	Vite, Nodemon, Dotenv
Getting Started
To get a local copy up and running, follow these simple steps.

Prerequisites
Node.js (v18.x or higher)

npm (v9.x or higher)

MongoDB URI (from a local instance or a cloud service like MongoDB Atlas)

Cloudinary account credentials (API Key, Secret, Cloud Name)

Backend Setup
Clone the repository:

Bash

git clone https://github.com/mohitkumar4/chattyServer.git
cd chattyServer/backend
Install NPM packages:

Bash

npm install
Create a .env file in the backend directory and add the following environment variables. Replace the placeholder values with your own credentials.

Code snippet

PORT=5001
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
NODE_ENV=development

# Cloudinary Credentials
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
Run the backend server:

Bash

npm run dev
The server will start on http://localhost:5001.

Frontend Setup
Navigate to the frontend directory from the project root:

Bash

cd ../frontend
Install NPM packages:

Bash

npm install
Run the frontend development server:

Bash

npm run dev
The React application will open in your browser at http://localhost:5173.

You should now have the full application running locally on your machine.
