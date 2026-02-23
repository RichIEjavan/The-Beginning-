Elderly Home Management System (EHMS)
A comprehensive web-based application for managing residents, staff, appointments, medical records, and billing in elderly care facilities. Developed as a full-stack project using PHP and MySQL, this system streamlines daily operations and improves resident care coordination.

https://img.shields.io/badge/License-MIT-yellow.svg
https://img.shields.io/badge/PHP-7.4+-blue
https://img.shields.io/badge/MySQL-5.7+-orange

📋 Features
User Authentication & Role-Based Access
Secure login with hashed passwords; four user roles: Admin, Doctor, Nurse, Receptionist. Each role has tailored permissions.

Resident Management
Add, edit, view, and discharge residents. Store personal details, emergency contacts, admission date, and room assignment.

Staff Management
Manage staff profiles (doctors, nurses, receptionists). Automatically creates corresponding user accounts.

Appointment Scheduling
Schedule appointments between residents and doctors, view daily/weekly lists, and perform check-in/check-out.

Medical Records
Maintain electronic health records per resident, including diagnoses, observations, and prescriptions. Accessible to clinical staff.

Billing & Invoicing
Create invoices for services, track payment status (Pending/Paid), and view outstanding balances.

Global Search
Quickly find residents or staff by name or room number across the entire system.

Responsive Dashboard
Role-specific dashboards display key metrics, upcoming appointments, and quick action buttons.

🛠️ Technologies Used
Technology	Purpose
PHP 7.4	Server-side logic, business layer
MySQL 5.7	Database management
HTML5 / CSS3	Frontend structure and styling
JavaScript	Basic client-side interactivity
XAMPP	Local development environment (Apache + MySQL)
bcrypt	Password hashing
Prepared Statements	SQL injection prevention
🚀 Installation
Prerequisites
XAMPP (or any Apache/MySQL/PHP stack)

Git (optional)

Steps
Clone or download the repository

bash
git clone https://github.com/yourusername/elderly-home-management.git
Or extract the ZIP file into your XAMPP htdocs folder, e.g., C:\xampp\htdocs\elderly_home\.

Start Apache and MySQL
Open the XAMPP Control Panel and start both services.

Create the database

Open phpMyAdmin: http://localhost/phpmyadmin

Create a new database named elderly_home

Import the SQL file located at sql/elderly_home.sql

Configure database connection
Edit config.php and update the database credentials if necessary (default: username root, password empty).

Access the application
Open your browser and go to http://localhost/elderly_home.
Log in using one of the default accounts:

Role	Username	Password
Admin	admin	password
Doctor	house	password
Nurse	nurse	password
Receptionist	reception	password
Note: Change default passwords immediately after first login for security.

📁 Project Structure
text
elderly_home/
│
├── index.php                # Login page
├── dashboard.php            # Main dashboard (role‑specific)
├── residents.php            # Resident management
├── staff.php                # Staff management (Admin only)
├── appointments.php         # Appointment scheduling
├── medical_records.php      # Medical records
├── billing.php              # Billing & invoicing
├── search.php               # Global search
├── logout.php               # Logout script
├── config.php               # Database configuration & session start
├── header.php / footer.php  # Common layout
│
├── css/
│   └── style.css            # Main stylesheet
│
├── js/
│   └── script.js            # Optional JavaScript
│
├── sql/
│   └── elderly_home.sql     # Database dump
│
├── docs/                     # Documentation
│   ├── SRS.md                # Software Requirements Specification
│   ├── SDD.md                # Software Design Document
│   ├── UserManual.md         # User manual
│   ├── TestingPlan.md        # Testing plan & results
│   └── ProjectReport.md      # Final project report
│
└── README.md                 # This file
📚 Documentation
All project documentation is available in the docs/ folder:

Software Requirements Specification (SRS) – Detailed functional and non‑functional requirements.

Software Design Document (SDD) – Architecture, database design, module breakdown.

User Manual – Step‑by‑step guide for end users.

Testing Plan – Test cases, results, and validation.

Project Report – Summary of the project, methodology, challenges, and lessons learned.

🖼️ Screenshots
(Placeholder – add actual screenshots of your application)

Login Page	Dashboard
https://screenshots/login.png	https://screenshots/dashboard.png
Residents List	Add Resident Form
https://screenshots/residents.png	https://screenshots/add-resident.png
🤝 Contributing
Contributions are welcome! If you'd like to improve the project, please:

Fork the repository.

Create a new branch (git checkout -b feature/YourFeature).

Commit your changes (git commit -m 'Add some feature').

Push to the branch (git push origin feature/YourFeature).

Open a Pull Request.

Please read CONTRIBUTING.md for more details.

📄 License
This project is licensed under the MIT License – see the LICENSE file for details.

📧 Contact
Author: Your Name

GitHub: @yourusername

Email: your.email@example.com

For questions or feedback, feel free to open an issue or contact me directly.

⭐ If you find this project useful, please give it a star!

