System Requirements — AnhQuoc_C5_Assignment

Summary
- This solution contains projects that target .NET Framework 4.8 and .NET 8. The API (server) uses a local SQL Server database (QuanLyThuVien) and runs on Kestrel / IIS Express during development.

Supported OS
- Development: Windows 10 (21H2+) or Windows 11

Required software
- .NET
  - .NET 8 SDK and runtime (for the Api project)
  - .NET Framework 4.8 Developer Pack and runtime (for the .NET Framework projects)
  - Database SQL Server

Ports and local URLs (development)
- Kestrel (Api project - launch profile):
  - HTTP: http://localhost:5037
  - HTTPS: https://localhost:7287
- IIS Express (if using IIS Express profile):
  - HTTP: http://localhost:25293
  - HTTPS (sslPort): 44339

Database connection (default)
- Default connection string file: AnhQuoc_Project/Api/appsettings.json
- Default connection string value:
  "Server=localhost;Initial Catalog=QuanLyThuVien;Integrated Security=True;Encrypt=True;Trust Server Certificate=True;"
- If your SQL Server instance uses a named instance or different host, update the ConnectionStrings:Default value in the Api appsettings.json before running.

Basic setup steps
1. Install required runtimes/SDKs and Visual Studio workloads listed above.
2. Restore NuGet packages (Visual Studio will auto-restore or use dotnet restore for .NET 8 projects).
3. Create the database:
   - Open SQL Server Management Studio (or use sqlcmd) and run the script: AnhQuoc_Database/05_QuanLyThuVien.sql. This creates the QuanLyThuVien database and seed data.
4. Update the API connection string if your SQL Server is not at localhost (see file above).
5. Open the solution AnhQuoc_C5_Assignment.sln in Visual Studio and start the Api project (choose the desired launch profile: https/http/IIS Express).

Verification commands
- Check installed .NET SDKs / runtimes:
  - dotnet --list-sdks
  - dotnet --list-runtimes
- Verify .NET Framework 4.8 is installed (PowerShell):
  - (Get-ItemProperty "HKLM:\\SOFTWARE\\Microsoft\\NET Framework Setup\\NDP\\v4\\Full").Release -ge 528040

Notes / troubleshooting
- Ensure SQL Server service is running and the account you use has permission to create and use the QuanLyThuVien database.