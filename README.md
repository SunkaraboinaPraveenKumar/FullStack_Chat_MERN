MERN Stack AI Chatbot

This is an AI Chatbot application inspired by ChatGPT, built using the MERN (MongoDB, Express, React, Node.js) stack with integration of OpenAI's GPT models.

The chatbot allows users to interact in real-time, stores chat messages in a database, and offers secure authentication features such as JWT tokens, HTTP-Only cookies, signed cookies, password encryption, and middleware chains for added security.

Features

AI-Powered Chatbot: Powered by OpenAI to provide human-like responses.

Real-Time Interaction: Users can engage with the chatbot in real-time.

Message Storage: Each user's chat history is stored in the database for retrieval and management.

User Authentication: Secure authentication using JWT tokens.

Cookie Security: Uses HTTP-only and signed cookies for added security.

Password Encryption: Passwords are hashed and stored securely in the database using bcrypt.

CRUD Operations: Users can retrieve and delete their chat messages.

Middleware Chains: Implements middleware for validation, authentication, and request processing.

Tech Stack

Frontend: React, Vite, Material-UI (MUI)

Backend: Node.js, Express

Database: MongoDB (Mongoose)

AI Integration: OpenAI GPT models

Authentication: JSON Web Tokens (JWT), bcrypt

Deployment: Vercel (Frontend) and Render (Backend)

Project Structure

Backend (/backend)

/dist/index.js: The main entry point for the backend, handling server setup and routing.

Authentication Middleware: Validates JWT tokens for secure access.

Chat API: Provides routes for retrieving and managing chat messages.

Environment Variables: Managed through dotenv.

Frontend (/frontend)

React with Vite: For building and serving the frontend quickly.

React-Router-Dom: Handles frontend routing for pages.

Axios: For API calls to the backend.

MUI: Provides UI components for styling.

Deployed Links

Frontend: https://menr-chat-fr-ont.vercel.app

Backend: https://mern-chat-backend-delta.vercel.app/api/v1/user/logout

Getting Started

Prerequisites

Ensure that you have the following installed on your local machine:

Node.js: Version 16+ is recommended.

MongoDB: Running locally or using a cloud service like MongoDB Atlas.

Vercel (Optional): For deploying the frontend.

Installation

Backend

Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/mern-chat-backend.git
Navigate to the backend folder:

bash
Copy code
cd backend
Install dependencies:

bash
Copy code
npm install
Set up the environment variables by creating a .env file in the root directory:

bash
Copy code
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
OPENAI_API_KEY=your_openai_api_key
Run the backend:

bash
Copy code
npm run dev
Frontend

Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/mern-chat-frontend.git
Navigate to the frontend folder:

bash
Copy code
cd frontend
Install dependencies:

bash
Copy code
npm install
Run the frontend:

bash
Copy code
npm run dev
Deployment

The frontend is deployed on Vercel and the backend is deployed on Render.

Frontend Deployment (Vercel)

Run the build command:

bash
Copy code
npm run build
Push to your Vercel project:

bash
Copy code
vercel --prod
Backend Deployment (Render)

Ensure your render-build script is set up in package.json.

Deploy on Render using their build commands.

Security Features

JWT Tokens: Used for user authentication.

HTTP-Only Cookies: Enhances security by preventing JavaScript access to cookies.

Signed Cookies: Adds an additional layer of security for cookie handling.

bcrypt: Passwords are hashed before being stored in the database.

API Endpoints

POST /api/v1/user/signup: Register a new user.

POST /api/v1/user/login: Log in an existing user.

GET /api/v1/user/logout: Log out the user (clears the session).

GET /api/v1/chat: Retrieve the user's chat history.

DELETE /api/v1/chat/: Delete a chat message by ID.

License

This project is licensed under the ISC License.

Contributions

Contributions are welcome! Feel free to open issues or submit pull requests to help improve the project.