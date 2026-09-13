# GoMart Application

## Retail Billing & Inventory Management System

GoMart Application is a Windows desktop-based retail billing and inventory management system developed using **C# Windows Forms**, **ADO.NET**, and **Microsoft SQL Server**.

The system is designed for a small retail store and provides role-based access, category and product management, seller/admin management, and billing functionality.

## Project Information

| Item | Details |
|---|---|
| Project Name | GoMart Application |
| Project Type | Desktop Application |
| Domain | Retail Billing & Inventory Management |
| Language | C# |
| Framework | .NET Framework 4.7.2 |
| UI | Windows Forms |
| Database | Microsoft SQL Server / LocalDB |
| Data Access | ADO.NET |
| Course | Object Oriented Programming 2 |
| Section | AA |

## Main Features

- Role-based login for Admin and Seller
- Category management
- Product management and validation
- Product search and category filtering
- Admin and seller management
- Retail billing and order total calculation
- Bill history storage
- SQL Server database integration through ADO.NET

## Application Modules

1. Login
2. Main/Home
3. Category Management
4. Product Management
5. Seller Management
6. Admin Management
7. Selling/Billing
8. About

## Architecture

**Windows Forms UI → DBConnect / ADO.NET → Microsoft SQL Server**

Stored procedures are used for several database write and management operations, while parameterized SQL commands are also used for database access.

## Database

The database contains five main tables:

- `tblAdmin`
- `tblSeller`
- `tblCategory`
- `tblProduct`
- `tblBill`

The product table references the category table through the category ID relationship.

### Database Files

- SQL setup: `Database/SQL_DB/GoMartDB_SQLServer_Setup.sql`
- Database package: `Database/GoMartDatabase.bacpac`

## How to Run

### Requirements

- Windows 10/11
- Visual Studio 2019 or later
- .NET Framework 4.7.2
- SQL Server LocalDB, Express, Developer, or another compatible SQL Server installation

### Database Setup

1. Open SQL Server Management Studio or another SQL Server database tool.
2. Run `Database/SQL_DB/GoMartDB_SQLServer_Setup.sql`.
3. Verify that the `GoMartDB` database is created.
4. Open `GoMartApplication.sln` in Visual Studio.
5. Check the connection string in `GoMartApplication/App.config`.
6. Build and run the application.

## Repository Contents

- `GoMartApplication/` — C# source code, Windows Forms, configuration, resources
- `Database/` — SQL setup script and database package
- `Documentation/Report/` — project report PDF
- `Documentation/Diagrams/` — project diagrams
- `Documentation/Screenshots/` — application screenshots

## Academic Project

Developed as an Object Oriented Programming 2 Final Term Project.

**Section:** AA
