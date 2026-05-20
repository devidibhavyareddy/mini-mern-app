# MERN Employee Management Application

## Project Overview

This project is a MERN Stack Employee Management Application developed using:

* MongoDB – Database
* Express.js – Backend framework
* React.js – Frontend library
* Node.js – Runtime environment

The application allows users to:

* Add new employees
* View employee details
* Edit employee information
* Delete employees
* Manage employee records using REST APIs
* Demonstrate state management using Zustand and React Context

# Project Architecture

Frontend (React + Vite + Tailwind CSS)
        ↓
REST API Calls (Axios / Fetch)
        ↓
Backend (Node.js + Express.js)
        ↓
MongoDB Database (Mongoose)

# Technologies Used

## Frontend

* React.js
* Vite
* Tailwind CSS
* React Router DOM
* Axios
* React Hook Form
* Zustand

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* CORS
* Nodemon

# Folder Structure

mern mini app/
│
├── backend/
│   ├── API/
│   │   └── Employeeapi.js
│   ├── Model/
│   │   └── Employeemodel.js
│   ├── package.json
│   └── server.js
│
├── frontend/
│   └── vite-project/
│       ├── src/
│       │   ├── components/
│       │   ├── contexts/
│       │   ├── stores/
│       │   ├── App.jsx
│       │   └── main.jsx
│       ├── package.json
│       └── vite.config.js
│
└── README.md

# Features

## Employee Management

* Create employee records
* View employee details
* Update employee information
* Delete employee records
* Fetch all employees from MongoDB

## Frontend Features

* React Router navigation
* Form handling
* State management with Zustand
* Responsive UI using Tailwind CSS
* API integration using Axios and Fetch

## Backend Features

* RESTful API design
* MongoDB database integration
* Error handling middleware
* CORS configuration
* Mongoose schema validation

# Database Schema

## Employee Model

{
  name: String,
  email: String,
  mobileno: String,
  designation: String,
  companyName: String
}

### Schema Validations

* Name is required
* Email is required and unique
* Mobile number is required and unique

# API Endpoints

## Base URL

/employee-api

## 1. Test API

### GET

/employee-api/test

### Response

Employee API working!

## 2. Create Employee

### POST

/employee-api/employees

### Request Body

{
  "name": "John Doe",
  "email": "john@example.com",
  "mobileno": "9876543210",
  "designation": "Developer",
  "companyName": "ABC Pvt Ltd"
}

## 3. Get All Employees

### GET

/employee-api/employees

## 4. Get Employee By ID

### GET

/employee-api/employees/:id

## 5. Update Employee

### PUT

/employee-api/employees/:id

## 6. Delete Employee

### DELETE

/employee-api/employees/:id

# Frontend Components

## RootLayout

Acts as the main layout wrapper for the application.

## Home Component

* Demonstrates Zustand state management
* Counter increment and decrement functionality

## CreateEmp Component

* Used to create a new employee
* Sends POST request to backend

## ListofEmp Component

* Displays all employees
* Includes View, Edit, and Delete operations

## EditEmployee Component

* Updates employee information
* Uses React Hook Form

## Employee Component

* Displays complete employee details

# State Management

## Zustand Store

The project uses Zustand for lightweight global state management.

### Features

* Counter state
* Increment functionality
* Decrement functionality

## React Context API

Also demonstrates Context API usage for shared state.

# Backend Explanation

## server.js

Responsible for:

* Creating Express server
* Connecting MongoDB database
* Configuring middleware
* Handling routes
* Starting server

## Employeeapi.js

Contains all employee-related API routes.

## Employeemodel.js

Defines MongoDB schema using Mongoose.

# Installation and Setup

## Step 1: Clone Repository

git clone <repository-url>

## Step 2: Backend Setup

Navigate to backend folder:

cd backend

Install dependencies:

npm install

Run backend server:

npm run dev

Server runs on:

http://localhost:4000

## Step 3: Frontend Setup

Navigate to frontend folder:

cd frontend/vite-project

Install dependencies:

npm install

Run frontend:

npm run dev

Frontend runs on:

http://localhost:5173

# Environment Variables

Create a `.env` file in backend folder.

DB_URL=mongodb://127.0.0.1:27017/employeeDB
PORT=4000

# Deployment

## Frontend Deployment

The frontend can be deployed using:

* Vercel
* Netlify

## Backend Deployment

The backend API can be deployed using:

* Render
* Railway
* Cyclic

# Sample API URLs

## Local Backend

http://localhost:4000/employee-api/employees

## Deployed Backend

https://mini-mern-app-xe26.onrender.com/employee-api/employees

# Learning Outcomes

Through this project, the following concepts were learned:

* MERN stack development
* REST API creation
* MongoDB CRUD operations
* React routing
* React hooks
* Zustand state management
* Form handling
* Backend integration
* Deployment basics

# Future Improvements

Possible future enhancements:

* Authentication and authorization
* JWT login system
* Search and filter employees
* Pagination
* Upload employee profile images
* Dashboard analytics
* Role-based access control
* Dark mode
* Email validation

# Conclusion

This MERN Employee Management Application is a complete full-stack CRUD project that demonstrates frontend and backend integration using modern web technologies. The project provides practical experience in building REST APIs, handling databases, managing frontend state, and creating responsive user interfaces.
