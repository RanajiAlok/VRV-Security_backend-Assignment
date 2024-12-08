#VRV Security Intern Assignment
This project is a comprehensive implementation of Authentication, Authorization, and Role-Based Access Control (RBAC) mechanisms as part of my internship assignment for VRV Security. The system ensures secure access control based on user roles and integrates Google OAuth for seamless authentication.

Table of Contents
Features
Technologies Used
Installation and Setup
API Endpoints
Google OAuth Configuration
Usage
Contributing
Features
User Registration: Allows users to register with a username, email, and password. Roles can be assigned during registration.
User Login: Users can log in using their email and password to receive a JWT for authenticated requests.
Role-Based Access Control (RBAC): Ensures that users have access to only those resources permitted by their role (e.g., Admin, User).
Google OAuth2 Login: Enables users to log in via their Google accounts, with JWT tokens generated upon successful login.
Protected Routes: Restricts access to specific API routes based on roles.
JWT Authentication: Secure token-based authentication using JSON Web Tokens.
Logout: Allows users to log out and invalidate their sessions.
Technologies Used
Backend:
Node.js
Express.js
Authentication:
Passport.js (Google OAuth)
JWT (JSON Web Tokens)
Database:
MongoDB with Mongoose
Password Encryption:
bcrypt.js
Frontend:
React.js
React Router
Version Control:
Git and GitHub
Installation and Setup
Prerequisites:
Install Node.js and npm (Node Package Manager).
Set up MongoDB locally or use a cloud-based MongoDB instance (e.g., MongoDB Atlas).
Step-by-Step Setup:
Clone the repository:

bash
Copy code
git clone https://github.com/YourUsername/VRV-Security-Intern-Assignment.git  
cd VRV-Security-Intern-Assignment  
Backend Setup:

bash
Copy code
cd server  
npm install  
Create a .env file in the root of the server directory and add the following:

env
Copy code
JWT_SECRET=your_jwt_secret  
GOOGLE_CLIENT_ID=your_google_client_id  
GOOGLE_CLIENT_SECRET=your_google_client_secret  
MONGO_URI=your_mongodb_uri  
SESSION_SECRET=your_session_secret  
PORT=your_port_number  
Start the backend server:

bash
Copy code
npm start  
Frontend Setup:

bash
Copy code
cd client  
npm install  
npm start  
Access the application:

Backend: http://localhost:5000/
Frontend: http://localhost:3000/
API Endpoints
Authentication Endpoints
POST /api/auth/register: Register a new user.
POST /api/auth/login: Log in with email and password.
GET /api/auth/google: Initiate Google OAuth login.
GET /api/auth/google/callback: Handle Google OAuth callback.
Role-Based Access Control
/user: Welcome message for users (accessible to "User" role only).
/admin: Welcome message for admins (accessible to "Admin" role only).
Google OAuth Configuration
Go to the Google Developers Console.
Create a new project and enable the Google Identity API.
Generate OAuth credentials (Client ID and Client Secret).
Add the GOOGLE_CLIENT_ID and GOOGLE_CLIENT_SECRET to your .env file.
Set the redirect URL to:
bash
Copy code
http://localhost:5000/auth/google/callback  
Usage
User Registration: Use the /register endpoint to create a new user.
Google Login: Log in using Google OAuth via /auth/google.
Admin Features: Admins can access the /admin route.
User Features: Users can access the /user route.
Contributing
Contributions, suggestions, and feature requests are welcome!

To Contribute:
Fork the repository.
Create a new branch:
bash
Copy code
git checkout -b feature/your-feature-name  
Make your changes and commit them:
bash
Copy code
git commit -m 'Add feature: your-feature-name'  
Push to your branch:
bash
Copy code
git push origin feature/your-feature-name  
Open a Pull Request on the main repository.
