# Elective Course Registration

A comprehensive web application for managing elective course registrations in engineering colleges. This system provides distinct interfaces for students to register for elective courses and faculty to manage course offerings and student enrollments.

**Live Demo**: [https://electivecourse.onrender.com/](https://electivecourse.onrender.com/)

## Features

### Student Features
- Secure login using USN and password (date of birth)
- Branch and semester selection
- Browse available elective courses with real-time availability status
- Register for preferred elective courses
- View registered course details

### Admin/Faculty Features
- Secure admin dashboard
- Create and manage elective courses by semester
- Edit course details (title, code, maximum enrollment limit)
- Track registration statistics
- Merge courses (combine registrations from one course to another)
- Export student registration data to Excel for each course

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript, EJS (Embedded JavaScript templates)
- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Authentication**: Passport.js, bcrypt
- **Additional Tools**: ExcelJS (for exports), dotenv (environment variables)

## Setup and Installation

### Prerequisites
- Node.js and npm installed
- MySQL database server

### Steps to Install and Run

1. Clone the repository:

        https://github.com/SanjayChoodamani/ElectiveCourse

        cd ElectiveCourse

2. Install dependencies:

        npm install 


3. Create a `.env` file with required configuration

4. Set up the database


5. Start the application:

        nodemon index.js

        or 

        node index.js


6. Access the application at `http://localhost:3000`

## Database Structure

The application uses several tables:
- `student`: Stores student information (USN, name, DOB, etc.)
- `login`: Stores login credentials
- `admin`: Stores admin/faculty login information
- `sem1` through `sem7`: Store course information for each semester
- `details`: Tracks student course registrations

## Usage Guide

### Student Login
1. Enter your USN (uppercase) and DOB as password
2. Select your branch and semester
3. Browse available elective courses
4. Select your preferred course
5. Submit your selection

### Faculty/Admin Login
1. Access the admin panel using credentials
2. Select semester to manage
3. Add new courses or edit existing ones
4. Export student registration data when needed
5. Use the merge feature to combine registrations if needed



Made with ❤️ for engineering students.