LIBRARY MANAGEMENT SYSTEM - RUNNING INSTRUCTIONS
==================================================

Prerequisites & Setup Steps
---------------------------
1. Install all required software in the SYSTEM_REQUIREMENTS.md file
2. Run the database script located in the 'Database' folder.
3. Open the 'appsetting.json' file in the API project, find the "ConnectionStrings" part, and in the default section, replace the following parts:
+ "Server=localhost": Replace the "localhost" value with the server name in the SQL Server connection dialog
+ "Integrated Security=True": If the authentication is SQL Server authentication, change it to false, and then add username and password information
4. Open the API project and then open the Library-Management-Application project

Default User Accounts
---------------------
- Administrator:
  Username: nhatminh
  Password: nhatminh

- Librarian:
  Username: hungvuong
  Password: hungvuong

Instruction Video
-----------------
Watch the setup video here:
[https://www.loom.com/share/647f62e0e7104195b3c7c457617040f](https://www.loom.com/share/647f62e0e7104195b3c7c457617040f8)

==================================================
Thank you for viewing my project!
