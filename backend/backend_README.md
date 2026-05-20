# Backend - MERN Employee Management System

## Overview

This is the backend server of the MERN Employee Management System developed using Node.js, Express.js, and MongoDB.

The backend handles:

- REST APIs
- Database operations
- CRUD functionality
- Employee data management

# Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- Nodemon
- CORS

# Backend Architecture

Client Request
      ↓
Express Server
      ↓
Routes / APIs
      ↓
Mongoose Models
      ↓
MongoDB Database

# Folder Structure

backend/
│
├── API/
│   └── Employeeapi.js
│
├── Model/
│   └── Employeemodel.js
│
├── package.json
├── server.js
└── .env

# API Explanation

## Employee APIs

The backend provides CRUD APIs for employee management.

### Base URL

/employee-api

# API Endpoints

## 1. Test Route

### GET

/employee-api/test

### Response

"Employee API working"

## 2. Create Employee

### POST

/employee-api/employees

### Request Body

{
  "name": "John",
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

# Database Schema

## Employee Model

const EmployeeSchema = new mongoose.Schema({
  name: {
    type: String,
    required: true
  },
  email: {
    type: String,
    required: true,
    unique: true
  },
  mobileno: {
    type: String,
    required: true,
    unique: true
  },
  designation: String,
  companyName: String
})

# Server Explanation

## server.js

Responsible for:

- Creating Express application
- MongoDB connection
- Middleware configuration
- API routing
- Server startup

# MongoDB Connection

The backend connects MongoDB using Mongoose.

## Example Connection

mongoose.connect(process.env.DB_URL)

# Middleware Used

## Express JSON

app.use(express.json())

## CORS

app.use(cors())

# Environment Variables

Create `.env` file inside backend folder.

DB_URL=mongodb://127.0.0.1:27017/employeeDB
PORT=4000

# Installation

## Step 1: Navigate to backend

cd backend

## Step 2: Install dependencies

npm install

## Step 3: Run backend server

npm run dev

Backend server runs on:

http://localhost:4000

# Backend Dependencies

{
  "express": "^4.x",
  "mongoose": "^8.x",
  "cors": "^2.x",
  "nodemon": "^3.x"
}

# Error Handling

The backend handles:

- Invalid requests
- Database connection errors
- Validation errors
- Duplicate email/mobile entries

# Deployment

## Backend Deployment Platforms

- Render
- Railway
- Cyclic

# Sample Backend URL

https://mini-mern-app-xe26.onrender.com

# Future Improvements

- JWT authentication
- Role-based access control
- Password encryption
- Logging system
- API documentation using Swagger
- Advanced validations

# Conclusion

The backend application provides a scalable REST API architecture for managing employee data using Node.js, Express.js, and MongoDB.
