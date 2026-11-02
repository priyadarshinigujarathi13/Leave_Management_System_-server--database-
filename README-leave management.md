# Leave Management System

A web-based Leave Management System built using **Node.js, Express.js, MySQL, HTML, CSS, and JavaScript**. The application helps manage employee leave applications and leave records through a simple, organized web interface.

## About the Project

The Leave Management System is designed to simplify the process of submitting, viewing, searching, and updating employee leave details. Instead of maintaining leave information manually, the application stores records in a MySQL database and provides a browser-based interface to manage them.

The project uses Express.js to handle HTTP requests and communicate with the MySQL database. The frontend provides pages for accessing the available leave-management operations.

## Features

- **Home Page:** Provides navigation to the available leave-management operations.
- **Apply for Leave:** Enter employee and leave details through a web form.
- **View Leave Records:** Retrieve and display stored leave applications.
- **Search Leave:** Find a leave record using the employee ID.
- **View Individual Record:** Display the details of a selected employee's leave record.
- **Update Leave Details:** Modify existing leave information.
- **Delete Leave Record:** Remove an existing leave record.
- **Database Integration:** Store and retrieve information using MySQL.
- **User-Friendly Interface:** A consistent interface for navigating the different pages.

## What I Would Like to Add

The following improvements are planned for future versions of the project:

- **Employee Login and Authentication:** Provide secure login for employees and administrators.
- **Role-Based Access:** Allow employees to apply for leave while managers or HR staff review requests.
- **Leave Approval Workflow:** Add Pending, Approved, and Rejected statuses for leave applications.
- **Leave Balance Management:** Track the number of leave days available to each employee.
- **Leave Calendar:** Display employee leave schedules in a calendar view.
- **Email Notifications:** Notify employees when their leave requests are approved or rejected.
- **Dashboard and Reports:** Show leave statistics, department-wise summaries, and monthly reports.
- **Form Validation:** Improve validation and error messages for invalid or incomplete entries.
- **Responsive Design:** Improve the interface for mobile phones, tablets, and desktop screens.
- **Improved Database Design:** Support multiple leave applications for each employee with a unique leave application ID.
- **Security Improvements:** Use environment variables for database credentials and add appropriate input validation and access controls.

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Structure of the web pages |
| CSS3 | Styling and responsive layout |
| JavaScript | Frontend interactions and API requests |
| Node.js | JavaScript runtime for the server |
| Express.js | Backend routes and HTTP request handling |
| MySQL | Database for employee and leave records |
| Git and GitHub | Version control and project hosting |

## Project Structure

```text
express/
├── app7leave.js
├── public/
│   ├── leave-style.css
│   ├── leave-home.html
│   ├── leave-insert.html
│   ├── leave-list.html
│   ├── leave-listOne.html
│   ├── leave-search.html
│   └── leave-update.html
└── README.md
```

## Prerequisites

Install the following before running the application:

- Node.js and npm
- MySQL Server
- A code editor such as Visual Studio Code
- A web browser

## Setup and Installation

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_REPOSITORY_FOLDER
```

Replace the placeholder with the actual GitHub repository URL.

### 2. Install dependencies

If the project has a `package.json` file:

```bash
npm install
```

Otherwise, install the dependencies used by the application, matching the MySQL package imported in `app7leave.js`.

### 3. Configure the database

Create the `leave_management` database in MySQL and ensure that the required tables and columns match the SQL queries in `app7leave.js`.

Do not publish database passwords or other secrets in the repository. Store credentials in environment variables.

### 4. Start the application

Run the server using:

```bash
node app7leave.js
```

### 5. Open the website

Open the following address in your browser:

```text
http://localhost:3000/
```

Make sure the MySQL server is running and the database connection is configured correctly.

## Backend API Overview

The application uses Express routes to manage leave records. The following endpoints describe the operations implemented in the current backend; verify their request fields and response formats against `app7leave.js`.

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/employees` | Retrieve employee details |
| GET | `/employee-ids` | Retrieve employee IDs |
| POST | `/leaves` | Create a leave record |
| GET | `/leaves` | Retrieve leave records |
| GET | `/leaves/:id` | Retrieve a record by employee ID |
| PUT | `/leaves/:id` | Update a record |
| DELETE | `/leaves/:id` | Delete a record |

## Learning Outcomes

Through this project, I explored:

- Building web pages using HTML, CSS, and JavaScript.
- Creating backend routes with Node.js and Express.js.
- Connecting a web application to a MySQL database.
- Performing CRUD operations: Create, Read, Update, and Delete.
- Sending HTTP requests between a frontend and backend.
- Organizing a multi-page web application.

## Future Scope

The project can be extended into a more complete employee leave-management platform with secure authentication, approval workflows, leave balance tracking, automated notifications, and analytical reports.

## Author

**Priya Darshini Gujarathi**

Student project developed for learning full-stack web development and database integration.

## License

This project is intended for educational purposes. Add a license if you plan to distribute or reuse the project publicly.