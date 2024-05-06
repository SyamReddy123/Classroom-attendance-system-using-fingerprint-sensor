# Classroom-attendance-system-using-fingerprint-sensor

## Overview:
This project implements a real-time attendance monitoring system using fingerprint authentication. It includes a web-based interface for managing users, devices, and attendance logs, as well as Arduino code for the ESP32 microcontroller to handle fingerprint scanning and communication with the server.

# Features:

## Web-based interface for administrators to:
Add, update, and remove users.
Add, update, and remove devices.
View attendance logs in real-time.

## ESP32 microcontroller functionality:
Fingerprint scanning using R307 Fingerprint Sensor.
Communication with the server for user verification.
Displaying messages on an OLED display based on verification results.

## Components:

### Web Interface:

PHP files for user management, device management, and attendance tracking.
HTML/CSS/JS for the user interface.
MySQL database for storing user information, devices, and attendance logs.
ESP32 Code:
Arduino code for fingerprint scanning and communication with the server.

## Setup Instructions:

### Web Server Setup:
Host the PHP files on a web server with PHP and MySQL support.
Import the provided SQL file to create the necessary database schema and tables.

## ESP32 Setup:
Open the Arduino IDE and upload the provided ESP32 code to the microcontroller.
Make sure to install the required libraries for fingerprint scanning and HTTP communication.

## Configuration:
Update the database connection settings in PHP files to match your MySQL server credentials.
Configure the ESP32 code with your web server's URL and other parameters as needed.

## Usage:

### User Management:
Access the user management interface (manage_users.php) to add, update, or remove users.
Users can be associated with specific departments and assigned fingerprint IDs.

## Device Management:
Use the device management interface (manage_devices.php) to add, update, or remove devices.
Each device should have a unique identifier and be associated with a department.

## Attendance Tracking:
Access the main interface (index.php) to view real-time attendance logs.
Attendance records include user names, timestamps, and device information.

## Fingerprint Scanning:
Users place their thumbs on the fingerprint sensor connected to the ESP32.
The ESP32 scans the fingerprint and communicates with the server for verification.
Messages are displayed on the OLED screen based on verification results.

## Security Considerations:
Implement proper input validation and sanitization in PHP to prevent SQL injection and other security vulnerabilities.
Use HTTPS to secure communication between the ESP32 and the web server.
Implement user authentication and authorization for web-based actions to prevent unauthorized access.

## Future Enhancements:
Implement additional features such as email notifications for attendance records.
Enhance user interface design for better user experience.
Improve error handling and logging for better debugging and troubleshooting.
