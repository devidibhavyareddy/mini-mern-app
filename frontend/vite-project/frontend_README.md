# Frontend - MERN Employee Management System

## Overview

This is the frontend part of the MERN Employee Management System developed using React.js and Vite. The application provides an interactive user interface for managing employee records.

# Technologies Used

- React.js
- Vite
- Tailwind CSS
- React Router DOM
- Axios
- React Hook Form
- Zustand
- JavaScript

# Features

## Employee Management

- Add new employees
- View employee details
- Edit employee information
- Delete employee records
- Display all employees

## UI Features

- Responsive design
- Navigation using React Router
- State management with Zustand
- Form validation
- API integration

# Project Structure

src/
│
├── components/
│   ├── RootLayout.jsx
│   ├── Home.jsx
│   ├── CreateEmp.jsx
│   ├── ListofEmp.jsx
│   ├── Employee.jsx
│   └── EditEmployee.jsx
│
├── contexts/
│   └── EmployeeContext.jsx
│
├── stores/
│   └── CounterStore.js
│
├── App.jsx
├── main.jsx
└── index.css

# Component Explanation

## RootLayout

Acts as the main layout wrapper and contains navigation.

## Home Component

- Demonstrates Zustand state management
- Counter increment and decrement example

## CreateEmp Component

Responsible for:

- Creating employee records
- Sending POST request to backend
- Handling form submissions

## ListofEmp Component

Responsible for:

- Fetching all employees
- Displaying employee list
- Delete functionality
- Navigation to edit and view pages

## Employee Component

Displays complete employee information.

## EditEmployee Component

Responsible for updating employee details using PUT API.

# Routing

The application uses React Router DOM for navigation.

## Routes

/create
/employees
/employees/:id
/edit/:id

# State Management

## Zustand Store

Used for global state management.

### Example Features

- Counter state
- Increment function
- Decrement function

# API Integration

The frontend communicates with backend APIs using Axios or Fetch.

## Example API URL

http://localhost:4000/employee-api/employees

# Installation

## Step 1: Navigate to frontend

cd frontend/vite-project

## Step 2: Install dependencies

npm install

## Step 3: Start development server

npm run dev

Frontend runs on:

http://localhost:5173

# Frontend Dependencies

{
  "react": "^18.x",
  "react-dom": "^18.x",
  "react-router-dom": "^6.x",
  "axios": "^1.x",
  "zustand": "^4.x"
}

# Future Improvements

- Authentication UI
- Search employees
- Pagination
- Dark mode
- Dashboard analytics
- Better form validation

# Conclusion

The frontend application provides a clean and responsive user interface for employee management using modern React development practices.
