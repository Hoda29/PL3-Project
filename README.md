# PL3-Project: School Management System

This repository hosts the **PL3-Project**, a comprehensive school management system designed to streamline various administrative and educational processes within an academic institution. The system is built primarily using **F#** and interacts with a **SQL** database for data persistence.

---

## Table of Contents

* [Features](#features)
* [Project Structure](#project-structure)
* [Technologies Used](#technologies-used)
* [Setup and Installation](#setup-and-installation)
* [Database Setup](#database-setup)
* [Usage](#usage)
* [Contributing](#contributing)
---

## Features

The PL3-Project provides essential functionality for managing a school environment. Based on the file names, the system likely includes:

* **User Authentication:** Secure login for different user roles (e.g., instructors, students, administrators). (`login_form.fs`)
* **Instructor Management:** Handle instructor data and operations. (`Instructor.fs`)
* **Section Management:** Manage classes, enrollments, and course assignments. (`section.fs`)
* **Core Application Logic:** Main application functionality and entry point. (`Program.fs`)
* **Database Integration:** SQL database interaction for data storage and retrieval. (`sms.sql`, `sms (1).sql`)

(If more features exist, please update this section with details like "Student Enrollment", "Course Scheduling", "Grade Management", etc.)

---

## Project Structure

```
.
├── Instructor.fs             # F# module for Instructor related logic
├── Program.fs                # Main application entry point and core logic
├── README.md                 # This README file
├── config.fsproj             # F# project configuration file
├── login_form.fs             # F# module for user authentication/login UI
├── section.fs                # F# module for Section (classes/courses) related logic
├── sms (1).sql               # SQL script (alternative/backup schema)
└── sms.sql                   # Main SQL database schema and data
```

---

## Technologies Used

* **F#**: Primary programming language
* **SQL**: Database management and persistence layer

(Optional: Add libraries/frameworks like `Suave`, `FSharp.Data`, etc. if used)

---

## Setup and Installation

To set up the project locally:

1. **Clone the Repository:**

```bash
git clone https://github.com/Hoda29/PL3-Project.git
cd PL3-Project
```

2. **Install .NET SDK:**
   Ensure you have the .NET SDK (which includes F#) installed. [Download here](https://dotnet.microsoft.com/).

3. **Restore Dependencies:**

```bash
dotnet restore
```

---

## Database Setup

This project uses a SQL database backend. Follow these steps:

1. **Create a Database:** Use your SQL server (SQL Server, PostgreSQL, MySQL, etc.) to create a new database.

2. **Run SQL Scripts:**
   Execute `sms.sql` to create tables and insert initial data. Optionally run `sms (1).sql` if needed.

3. **Update Connection String:**
   In `Program.fs` or config file, locate and update the connection string:

```fsharp
let connectionString = "Data Source=your_server;Initial Catalog=your_database;User ID=your_user;Password=your_password;"
```

---

## Usage

After setup:

1. **Build the Application:**

```bash
dotnet build
```

2. **Run the Application:**

```bash
dotnet run
```

This will launch the School Management System. (Please add details for logging in or using the UI if applicable.)

---

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a feature branch:

```bash
git checkout -b feature/YourFeatureName
```

3. Make your changes.
4. Commit your changes:

```bash
git commit -m 'Add new feature'
```

5. Push to your fork:

```bash
git push origin feature/YourFeatureName
```

6. Open a Pull Request.

