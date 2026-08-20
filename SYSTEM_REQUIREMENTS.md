================================================================================
                       SYSTEM REQUIREMENTS & SETUP
                       AnhQuoc_C5_Assignment
================================================================================

1. REQUIRED SOFTWARE
--------------------------------------------------------------------------------
* .NET 8 SDK
  - Download URL: https://dotnet.microsoft.com/en-us/download/dotnet/8.0

* .NET Framework 4.8
  - Included natively / available on Windows 10

* Microsoft SQL Server
  - Required for local database hosting


2. INSTALLATION VERIFICATION
--------------------------------------------------------------------------------
To check if the .NET 8 SDK is installed:

  1. Open Command Prompt or PowerShell.
  2. Run the following command:

     dotnet --list-sdks

  3. Verification:
     If the command output contains an entry starting with '8.0' (or a higher
     version number), the .NET 8 SDK is installed and ready for use.


3. TROUBLESHOOTING & NOTES
--------------------------------------------------------------------------------
* SQL Server Service:
  Ensure the Microsoft SQL Server service (MSSQLSERVER or SQLEXPRESS) is 
  running prior to starting the application.

================================================================================