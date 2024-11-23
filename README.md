# RBAC-project


Role-Based Access Control (RBAC) Application

This project is a Role-Based Access Control (RBAC) system built using React.js and JSON Server. It allows for role-based authentication and authorization, enabling different views and functionalities for Admin and User roles. The application includes features like user and role management, dynamic permissions, and secure login.

Features
User Management
View, add, edit, and delete users.
Assign roles and manage user activation status.
Prevent inactive users from logging in.
Role Management
Define and edit roles.
Assign permissions (Read, Write, Delete) to roles dynamically.
Permissions dictate access to features like Add Spots, Explore, and Delete Spots.
Authentication & Authorization
Secure login with hashed passwords (using bcryptjs).
Differentiated dashboards for Admin and User roles.
Unauthorized users are restricted with appropriate alerts.
Spot Management
Add, view, and delete tourist spots.
Manage spots based on role-specific permissions.
Custom API Simulation
Uses json-server to simulate API calls for CRUD operations.
All data (users, roles, spots) is managed via JSON Server.

Getting Started
Prerequisites
Node.js installed
npm (Node Package Manager)

1. clone project

2. Install dependencies: npm install

3. Start json server using : npx json-server --watch db.json --port 5000

4. Run the react app using : npm start

Usage
Admin Features
Login with admin credentials--> email:"admin123@gmail.com"
				                        password:"achal123"
Navigate to:
User Management: Manage user details,assign roles, and activation.
If user is inactive then that user cannot login
Role Management: Assign permissions and create new role.
Add Spots: Add new tourist spots (Permission based)

User Features
Login with valid user credentials--> email:"mark12@gmail.com"
				                             password:"mark123"
Or you can create new user using registration form

Access:
Home: View personalized welcome message.
Explore: Browse tourist spots (based on Read permission).
