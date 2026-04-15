# KabeloMoloko-Portfolio
🚗 Car Voting System

A client-server based application that allows users to vote for their favourite cars in a secure and structured environment.

📖 Overview

The Car Voting System is a distributed application where users connect through a client interface to vote for their preferred cars. The system ensures that each user can only vote once while maintaining accurate and secure data storage.

The server manages all client requests, processes votes, and communicates with the database to store and retrieve information efficiently.

🧩 Features
🔐 User authentication (login system)
🚗 View available cars
🗳️ Cast a vote
✅ One-user-one-vote enforcement
⚡ Real-time vote processing
💾 Secure database storage
🏗️ System Architecture
[ Client (GUI) ]  <---->  [ Server ]  <---->  [ Database ]
   (Swing)              (Java Sockets)        (MySQL)
Client Layer: Handles user interaction (Java Swing)
Server Layer: Processes requests and business logic
Database Layer: Stores users, cars, and votes
👨‍💻 My Role

I was responsible for integrating the server with the database using JDBC.

Configured database connection (URL, username, password)
Integrated JDBC driver in NetBeans IDE
Implemented SQL queries for:
User authentication
Retrieving car data
Recording votes
Updating vote counts
Used PreparedStatement to prevent SQL injection
Implemented exception handling for reliability
Ensured proper resource management (closing connections, statements, result sets)
🛠️ Technologies Used
Java
NetBeans IDE
Socket Programming (ServerSocket, Socket)
JDBC (Java Database Connectivity)
MySQL
Java Swing (GUI)
⚙️ How It Works
User launches the client application
User logs in or registers
Client sends request to server
Server validates user using the database
User selects a car and submits a vote
Server records the vote and updates results
Confirmation is sent back to the client
📦 Setup Instructions
Prerequisites
Java JDK installed
MySQL installed
NetBeans IDE
Steps

Clone the repository:

git clone https://github.com/your-username/car-voting-system.git
Open the project in NetBeans
Set up the MySQL database:
Create database
Import/create tables (Users, Cars, Votes)

Update database connection in code:

String url = "jdbc:mysql://localhost:3306/your_db";
String user = "root";
String password = "your_password";
Run the server
Run the client application
📌 Future Improvements
🌐 Convert to web application (Spring Boot + React)
🔒 Add password hashing (bcrypt)
📊 Admin dashboard for managing cars
📱 Mobile app version
📈 Live voting results visualization
📄 License

This project is for educational purposes.
