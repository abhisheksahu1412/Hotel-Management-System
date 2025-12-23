
# Hotel Management System (Java + JDBC + MySQL)
📝 Project Description

This is a console-based Hotel Management System developed using Java, JDBC, and MySQL.
The application allows hotel staff to manage room reservations efficiently.

🚀 Features

1️⃣ Reserve a room
2️⃣ View all reservations
3️⃣ Update reservation details
4️⃣ Delete a reservation
5️⃣ Get room number using reservation ID
6️⃣ Secure database connection using JDBC

🛠 Technologies Used

Java (JDK 8+)

JDBC

MySQL Database

IntelliJ IDEA / VS Code

Git & GitHub

🗂 Database Structure

Database Name: hotel_db
Table Name: reservations

CREATE DATABASE hotel_db;
USE hotel_db;

CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100),
    room_number INT,
    contact_number VARCHAR(15),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

⚙️ Project Configuration

Update database credentials in Main.java:

private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "YOUR_PASSWORD";

▶️ How to Run the Project

Clone the repository

Import project into IDE

Add MySQL JDBC Driver

Run Main.java

📷 Sample Output
HOTEL MANAGEMENT SYSTEM
1. Reserve a room
2. View Reservations
3. Update Reservations
4. Delete Reservations
5. Get Room Number
0. Exit

📌 Key Concepts Used

JDBC Connection

SQL CRUD Operations

Exception Handling

Loops & Switch Case

Modular Programming

👨‍💻 Author

Abhishek Sahu
B.Tech (Computer Science)

✅ 2️⃣ Step-by-Step: Dependencies Download (MySQL JDBC Driver)
🔹 Step 1: Download MySQL Connector/J

1️⃣ Open browser
2️⃣ Search: MySQL Connector/J download
3️⃣ Go to official MySQL site
4️⃣ Download Platform Independent (ZIP)

🔹 Step 2: Extract ZIP File

Extract folder

You will get file like:

mysql-connector-j-8.0.xx.jar

🔹 Step 3: Add JDBC Jar to Project
🔸 In IntelliJ IDEA

1️⃣ Right click project
2️⃣ Open Project Structure
3️⃣ Click Libraries
4️⃣ Add JAR file
5️⃣ Apply → OK

🔸 In VS Code

1️⃣ Create folder: lib
2️⃣ Paste .jar file inside lib
3️⃣ Right click jar → Add to Classpath

🔹 Step 4: Verify Driver

Your code already has:

Class.forName("com.mysql.cj.jdbc.Driver");


