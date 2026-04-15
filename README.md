# KabeloMoloko-Portfolio
# Car Voting System

A client-server based car voting system that allows users to vote for their preferred cars through a centralized application. Users connect via a client interface, log in, view available cars, and cast their votes. The server handles all client requests, ensures users can only vote once, and securely manages all voting data with a MySQL database.

---

## Project Overview

This project demonstrates a complete client-server architecture with database integration. It was developed to provide a secure, reliable platform for conducting car preference polls where each user is allowed exactly one vote.

---

## My Role

I was responsible for **connecting the server to the database using JDBC** and ensuring seamless communication between the two components.

### Key Contributions:
- Configured database connection with connection string, username, and password
- Integrated JDBC driver within **NetBeans IDE**
- Wrote and executed SQL queries for:
  - User authentication
  - Retrieving car data
  - Recording votes
  - Updating vote counts
- Used **PreparedStatement** to prevent SQL injection attacks
- Implemented robust **exception handling** for connection failures and query issues
- Ensured proper closure of database resources to maintain system performance

My role was essential for reliable data storage, vote accuracy, and seamless server-database interaction.

---

## Technologies Used

| Category | Technology |
|----------|------------|
| Language | Java |
| IDE | NetBeans |
| Networking | Socket Programming (ServerSocket, Socket) |
| Database Connectivity | JDBC |
| Database | MySQL |
| GUI | Java Swing |

---

## Database Schema

The system uses three main tables:

- **Users** – Stores user credentials and voting status
- **Cars** – Stores car details (ID, name, model, current vote count)
- **Votes** – Logs each vote with user ID, car ID, and timestamp

---

## Installation Instructions

### Prerequisites

- Java JDK installed
- MySQL installed and running
- NetBeans IDE (or any Java IDE)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/car-voting-system.git
Open the project in your IDE (NetBeans recommended)

Set up the database

Create a MySQL database (e.g., car_voting_db)

Create the required tables: Users, Cars, Votes

(Optional) Insert sample car data

Update database credentials in the server code

java
String url = "jdbc:mysql://localhost:3306/your_db";
String user = "root";
String password = "your_password";
Run the server application first

Run the client application (one or multiple instances)

How It Works
Client connects to the server via socket connection

User logs in – credentials verified against the database

Car list is displayed – retrieved from the Cars table

User votes for a car

Server checks if user has already voted (using Votes table)

If eligible, vote is recorded and car's vote count is incremented

Updated results can be viewed by clients
