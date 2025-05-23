----------------------🛠️ Room Management System – Instruction Manual------------------------
This manual provides step-by-step instructions to set up, configure, and operate the Room Management System on a local or networked server using XAMPP, PHP, MySQL, and HTML.

--------- System Requirements ----------
Operating System: Windows, macOS, or Linux

Software Stack:

XAMPP (includes Apache, MySQL, PHP)

Web Browser (Chrome, Firefox, etc.)

Code Editor (e.g., VS Code or Sublime Text)

---------- Installation Steps ----------
1. Install XAMPP
Download and install XAMPP from apachefriends.org.

Open XAMPP Control Panel.

Start Apache and MySQL modules.

2. Set Up the Project Directory
Place the Room Management System files in the htdocs directory:

makefile
Copy
Edit
C:\xampp\htdocs\room-management-system
3. Import the Database
Open http://localhost/phpmyadmin

Click on Databases > Create a new database (e.g., room_db)

Click Import > Choose your .sql file > Click Go

4. Configure Database Connection
Locate the config.php (or similar) file in your project

Update with your local DB credentials:

php
Copy
Edit
$host = "localhost";
$user = "root";
$password = "";
$database = "room_db";
🧭 Navigating the System
🔐 Login Page
Visit http://localhost/room-management-system

Enter admin or user credentials to log in

----------- Dashboard ----------
View room availability, booking statistics, and recent activity

---------- Rooms ----------
Add, edit, or remove room details (e.g., capacity, type, facilities)

---------- Bookings ----------
Create new bookings

View and manage current reservations

Automatically detect booking conflicts

---------- Users ----------
Admin can add/remove users and assign roles (Admin, Staff, Users)

---------- System Management -----------
Add New Room
Navigate to Rooms

Click Add Room

Fill out room details and save

Book a Room
Navigate to Bookings

Click New Booking

Select room, time, and user details

Confirm booking

---------- Add a Usern ----------
Go to Users

Click Add User

Assign role and credentials

---------- Troubleshooting ----------
Problem	Solution
Apache/MySQL not starting	Ensure ports 80 and 3306 are free (check Skype, etc.)
Database connection error	Verify config.php and DB credentials
Blank page loading	Enable PHP error reporting or check Apache logs
Styles not loading	Check if paths to CSS/JS files are correct

---------- Support & Maintenance ----------
Admin Access: For recovering passwords or user issues

Backups: Regularly export your database from phpMyAdmin

Security: Always validate inputs to prevent SQL injection
