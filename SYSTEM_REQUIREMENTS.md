System Requirements — AnhQuoc_C5_Assignment

Required software
- .NET 8 SDK and runtime (link download: https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- .NET Framework 4.8 (Available on Windows 10)
- Microsoft SQL Server

Basic setup steps
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