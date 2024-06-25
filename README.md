# Library Management System

## Overview

Welcome to the Library Management System! This project is a comprehensive solution designed to manage the operations of a library. The system is built using Java and JSP (JavaServer Pages) for the backend and front-end functionalities, respectively. The data is managed using a MySQL database. This document provides an overview of the system's functionalities, setup instructions, and other relevant information.

## Features

### User Management
- **User Registration**: Allows new users to register by providing their details.
- **User Login**: Registered users can log in using their credentials.
- **User Profile**: Users can view and update their profile information.
- **Password Management**: Users can change their password and recover a forgotten password.

### Book Management
- **Add Books**: Administrators can add new books to the library's inventory.
- **Update Books**: Administrators can update the details of existing books.
- **Delete Books**: Administrators can remove books from the inventory.
- **View Books**: Users can view a list of all available books in the library.
- **Search Books**: Users can search for books by title, author, genre, or ISBN.

### Borrowing Management
- **Issue Books**: Administrators can issue books to users.
- **Return Books**: Administrators can process the return of books.
- **View Borrowed Books**: Users can view the list of books they have borrowed.
- **Due Date Management**: The system tracks due dates and notifies users of upcoming due dates.

### Notifications
- **Email Notifications**: Users receive email notifications for book issues, returns, and due dates.
- **System Alerts**: The system provides alerts for overdue books.

## Prerequisites

Before you begin, ensure you have met the following requirements:
- Java Development Kit (JDK) 8 or higher installed on your machine.
- Apache Tomcat server 8.0 or higher.
- MySQL database server.
- MySQL JDBC Driver.
- An IDE like Eclipse or IntelliJ IDEA for development.

## Installation

### Step 1: Clone the Repository

Clone the repository to your local machine using the following command:
```bash
git clone https://github.com/yourusername/library-management-system.git
```

### Step 2: Set Up the MySQL Database

1. Start your MySQL server.
2. Create a new database named `library_db`.
3. Execute the SQL script `library_db.sql` provided in the `sql` directory to set up the required tables.

### Step 3: Configure the Database Connection

1. Open the project in your IDE.
2. Navigate to the `src/main/resources` directory.
3. Open the `db.properties` file and configure your MySQL database connection details:
```properties
db.url=jdbc:mysql://localhost:3306/library_db
db.username=root
db.password=yourpassword
```

### Step 4: Deploy the Application

1. Build the project using your IDE.
2. Deploy the `library-management-system.war` file to your Apache Tomcat server.
3. Start the Tomcat server. 

### Step 5: Access the Application

Open your web browser and navigate to `http://localhost:8080/library-management-system`.

## Usage

### Admin Login

1. Go to the admin login page.
2. Use the default admin credentials:
   - **Username**: admin
   - **Password**: admin123
3. Change the password after the first login.

### User Registration

1. Go to the user registration page.
2. Fill in the required details and submit the form.
3. Verify your email to activate your account.

### Borrowing Books

1. Log in to your user account.
2. Browse or search for books.
3. Select a book and click on "Borrow".
4. Check your email for borrowing confirmation.

## Contribution

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

If you have any questions or feedback, please contact us at TheTusharA1@gmail.com.

Thank you for using the Library Management System!
