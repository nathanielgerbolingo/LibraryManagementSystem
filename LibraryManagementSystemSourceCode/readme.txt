===========================================
LIBRARY MANAGEMENT SYSTEM
===========================================

===========================================
QUICK SETUP GUIDE
===========================================

1. INSTALL PREREQUISITES:
   - Java JDK 8 or higher
   - MySQL Server 5.7 or higher
   - Download from official websites

2. DATABASE SETUP:
   a. Open MySQL Command Line
   b. Run: CREATE DATABASE library_db;
   c. Run: USE library_db;
   d. Run: SOURCE database/library_db.sql;

3. CONFIGURE CONNECTION:
   Edit: src/librarysystem/DatabaseConnection.java
   Change: USER = "root" and PASSWORD = "yourpassword"

4. RUN APPLICATION:
   Windows: Double-click run.bat
   OR
   Command: java -cp "src;lib/*" librarysystem.LibraryManagementSystem

===========================================
DEFAULT LOGIN CREDENTIALS
===========================================

ADMIN ACCOUNT:
Username: admin
Password: 1234
Role: Administrator

STUDENT ACCOUNTS:
Username: nathaniel
Password: 1234
Role: Student

Username: marb
Password: 5678
Role: Student

===========================================
FEATURES
===========================================

- Role-based access (Admin/Student)
- Reputation-based borrowing system
- Late return penalties (-5 reputation)
- Book management (Add/Remove/Update)
- User management with account locking
- Transaction history logging
- Real-time book availability
- Data export to CSV

===========================================
REPUTATION SYSTEM
===========================================

80-100 points: EXCELLENT (3 books max)
50-79 points: GOOD (2 books max)
0-49 points: FAIR (1 book max)

Late returns: Automatic -5 points penalty
Admin can manually adjust reputations

===========================================
TROUBLESHOOTING
===========================================

PROBLEM: "Cannot connect to database"
SOLUTION: Ensure MySQL service is running

PROBLEM: "Class not found"
SOLUTION: Add mysql-connector-java-8.0.33.jar to lib/ folder

PROBLEM: "Access denied"
SOLUTION: Check MySQL username/password in DatabaseConnection.java

===========================================
CONTACT
===========================================

For support or questions:
Email: your.email@example.com
GitHub: https://github.com/yourusername

===========================================
ENJOY USING THE SYSTEM!
===========================================