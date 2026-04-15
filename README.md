# KabeloMoloko-Portfolio
# 🚗 Car Voting System

## 📖 Description
The Car Voting System is a client-server based application that allows users to vote for their preferred cars through a centralized platform. Users connect to the system via a client interface where they can log in, view a list of available cars, and cast their vote.

The server handles all client requests, processes votes, enforces the rule that each user can only vote once, and communicates with the database to store and retrieve information. This ensures that all voting data is managed securely and consistently.

The system is developed using Java, with socket programming enabling communication between the client and server. JDBC is used to connect the server to a MySQL database, which stores user information, car details, and voting records. A graphical user interface built using Java Swing allows users to interact with the system easily.

---

## ⚙️ Installation Instructions

### Prerequisites
- Java JDK installed
- MySQL installed
- NetBeans IDE (or any Java IDE) installed 

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-voting-system.git
Open the project in your IDE (e.g., NetBeans)
Set up the database:
Create a MySQL database
Create the required tables: Users, Cars, Votes

Update the database connection in the code:

String url = "jdbc:mysql://localhost:3306/your_db";
String user = "root";
String password = "your_password";
Run the server application
Run the client application
▶️ Usage Instructions
Launch the client application
Register a new account or log in
View the list of available cars
Select a car to vote for
Submit your vote
Receive confirmation (only one vote per user is allowed)
