LIBRARY MANAGEMENT SYSTEM - RUNNING INSTRUCTIONS
==================================================

Prerequisites & Setup Steps
---------------------------
1. Install all required software in the SYSTEM_REQUIREMENTS.md file

2. Run the database script located in the 'Database' folder.

3. Open the 'appsetting.json' file in the API project, find the "ConnectionStrings" part, and in the default section, replace the following parts:
+ "Server=localhost": Replace the "localhost" value with the server name in the SQL Server connection dialog
+ "Integrated Security=True": If the authentication is SQL Server authentication, change it to false, and then add username and password information
4. Open the API project:
 Step 1: Open PowerShell and navigate to the API project folder (Library-Management-Application\API)
 Step 2: Run this command "$env:ASPNETCORE_URLS = "https://localhost:7287;http://localhost:5037""
 Step 3: Run the command ".\Api.exe"
5. Open the Library-Management-Application project

5. Open the Library_management_guidance.pdf file to learn how to use my application

Default User Accounts
---------------------
- Administrator:
  Username: nhatminh
  Password: nhatminh

- Librarian:
  Username: hungvuong
  Password: hungvuong



==================================================
Thank you for viewing my project!
