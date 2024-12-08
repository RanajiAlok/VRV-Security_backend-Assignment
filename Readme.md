# **VRV Security Intern Assignment**

This project is a comprehensive implementation of **Authentication**, **Authorization**, and **Role-Based Access Control (RBAC)** mechanisms, completed as part of my internship assignment for **VRV Security**. The system ensures secure access control based on user roles and integrates **Google OAuth** for seamless authentication.

---

## **Table of Contents**
1. [Features](#features)  
2. [Technologies Used](#technologies-used)  
3. [Installation and Setup](#installation-and-setup)  
4. [API Endpoints](#api-endpoints)  
5. [Google OAuth Configuration](#google-oauth-configuration)  
6. [Usage](#usage)  
7. [Contributing](#contributing)  

---

## **Features**

- **User Registration**: Allows users to register with a username, email, and password. Roles can be assigned during registration.  
- **User Login**: Users can log in using their email and password to receive a JWT for authenticated requests.  
- **Role-Based Access Control (RBAC)**: Ensures that users have access to only those resources permitted by their role (e.g., Admin, User).  
- **Google OAuth2 Login**: Enables users to log in via their Google accounts, with JWT tokens generated upon successful login.  
- **Protected Routes**: Restricts access to specific API routes based on roles.  
- **JWT Authentication**: Secure token-based authentication using JSON Web Tokens.  
- **Logout**: Allows users to log out and invalidate their sessions.  

---

## **Technologies Used**

### **Backend:**
- Node.js  
- Express.js  

### **Authentication:**
- Passport.js (Google OAuth)  
- JWT (JSON Web Tokens)  

### **Database:**
- MongoDB with Mongoose  

### **Password Encryption:**
- bcrypt.js  

### **Frontend:**
- React.js  
- React Router  

### **Version Control:**
- Git and GitHub  

---

