# Employee Review System (ERS)

## Overview

The Employee Review System (ERS) is a web application that provides functionality for managing user reviews and feedback within an organization. The application is built using Node.js with Express, EJS for templating, and Bootstrap for styling. It supports different user roles including Admin and Employee, with separate dashboards and functionalities for each role.

## Features

- **Admin Dashboard**: Allows administrators to view all employees, assign reviews, and manage employee records (edit or delete).
- **Employee Dashboard**: Enables employees to view reviews assigned to them and feedback given to them by others.
- **Authentication**: Users can sign up and log in to access their respective dashboards.
- **Responsive Design**: The application is designed to be responsive and work well on various devices.

## Technologies Used

- **Node.js**: Server-side JavaScript runtime.
- **Express**: Web application framework for Node.js.
- **EJS**: Embedded JavaScript templating.
- **Bootstrap**: CSS framework for responsive design.
- **Passport**: Middleware for authentication.

## Installation

### Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

### Clone the Repository

```bash
git clone https://github.com/shivamp1998/ers.git
cd ers
```

### Install the dependencies

```bash
npm install
```

### Configuration
Create a .env file in the root directory and add your environment variables:

PORT=3000
SESSION_SECRET=your_secret_key
MONGO_URI=your_mongodb_connection_string


### Run the Application

Start the server with the following command:

```bash
npm start
```

## Usage

### Authentication

1. **Sign Up**: Users can sign up with their email, name, role (Admin or Employee), and password.
2. **Log In**: Users can log in with their email and password.

### Admin Dashboard

- **View Employees**: Admins can view a list of all employees.
- **Assign Reviews**: Admins can assign reviews to employees.
- **Manage Employees**: Admins can edit or delete employee records.

### Employee Dashboard

- **View Assigned Reviews**: Employees can view reviews assigned to them.
- **Submit Reviews**: Employees can submit feedback for other employees.
- **View Feedbacks**: Employees can see feedback received from others.

## Project Structure

- `app.js`: Main application file that sets up the Express server and middleware.
- `views/`: Contains EJS templates for rendering HTML pages.
- `routes/`: Contains route handlers for different endpoints.
- `models/`: Contains Mongoose models for MongoDB collections.
- `public/`: Contains static assets like images and stylesheets.
- `middleware/`: Contains custom middleware for authentication and authorization.