# 🏠 Roommate Finder

## 📘 Overview
**Roommate Finder** is a JavaFX-based desktop application designed to simplify the process of finding compatible roommates.  
The project provides a secure and user-friendly platform where users can create roommate listings, browse available postings, and apply detailed filters to find ideal living partners.  

Built with **Java**, **JavaFX**, and **MySQL**, the system combines intuitive UI design with reliable backend logic, ensuring a smooth user experience and efficient data management.

---

## ✨ Key Features
- 🔐 **Secure Authentication** – Login, signup, and password reset using OTP verification and password hashing.  
- 🏡 **Roommate Posting** – Create detailed roommate listings with lifestyle preferences, location, and rent details.  
- 🔎 **Dynamic Filtering** – Filter available listings by location, budget, room type, and other preferences.  
- 👤 **Profile Management** – Manage your own posts and view user-specific property details.  
- 💾 **Database Integration** – MySQL database connectivity using JDBC for storing and retrieving listings.  
- 🪟 **Interactive GUI** – Clean and responsive interface designed using JavaFX and Scene Builder.  

---

## 🧱 Tech Stack
| Layer | Technology |
|-------|-------------|
| **Frontend** | JavaFX (FXML, Scene Builder) |
| **Backend** | Java, JDBC |
| **Database** | MySQL (via SQL Workbench) |
| **IDE** | Eclipse |
| **Libraries** | BCrypt for password hashing, JavaFX SDK |

---

## ⚙️ Setup and Installation

### Prerequisites
Make sure the following are installed:
- [Eclipse IDE](https://www.eclipse.org/downloads/)
- [JavaFX SDK](https://openjfx.io/)
- [MySQL](https://dev.mysql.com/downloads/)
- [MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/)

---

### 1️⃣ Configure JavaFX in Eclipse
1. Download and extract the JavaFX SDK.  
2. In Eclipse, right-click your project → **Properties → Java Build Path → ModulePath → Add External JARs...**  
3. Select all JARs from the `lib` folder inside your JavaFX SDK directory.  
4. Apply changes and close.

---

### 2️⃣ Add MySQL Connector
1. Download **MySQL Connector/J** from the official website.  
2. In Eclipse:  
   `Properties → Java Build Path → Add External JARs... → Select the connector JAR file`.  
3. Apply and close.

---

### 3️⃣ Configure VM Arguments
In **Run Configurations → Arguments → VM Arguments**, add:
  ```
  --add-modules javafx.controls,javafx.fxml
  ```

---

### 4️⃣ Set Up the Database
1. Open **MySQL Workbench**.  
2. Create a new database schema (e.g., `roommatefinder_db`).  
3. Import the provided database dump file (`.sql`).  
4. Update the database credentials in your Java code if necessary:
   ```java
   String url = "jdbc:mysql://localhost:3306/roommatefinder_db";
   String user = "root";
   String password = "yourpassword";

---

### 5️⃣ Run the Application

1. Ensure all dependencies are configured.
2. Right-click on the main class → Run As → Java Application.
3. The Roommate Finder UI should launch successfully.

---
## 🧠 Implementation Overview

### 🔒 Authentication Module
- Implements user registration and login.  
- Passwords hashed with **BCrypt** for security.  
- OTP-based email verification for signup and password reset.  

---

### 🏡 Roommate Post Module
- Users can create listings with property details, location, rent, and preferences.  
- Data stored in the **MySQL database** using **JDBC**.  

---

### 🔍 Filtering & Search
- Filters results dynamically by multiple criteria using **SQL queries**.  
- Users can clear filters to reset search results.  

---

### 👤 User Profile
- Displays user-specific posts and profile information.  
- Allows easy management of created listings.  

---

### 🧱 Object-Oriented Design
- Uses **class inheritance**, **interfaces**, and **polymorphism** for modularity.  
- Applies **collections**, **maps**, and **recursion** for efficient data handling.  

---

### 📊 Results
- The application provides a **responsive** and **visually clean interface**.  
- Filtering and database connectivity perform efficiently under multiple search conditions.  
- Successfully enables **secure user interactions** and **profile-based roommate matching**.  

