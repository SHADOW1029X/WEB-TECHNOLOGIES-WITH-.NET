# WEB-TECHNOLOGIES-WITH-.NET
EXPENSE TRACKER
Description
Expense Tracker is a web application built using ASP.NET Core MVC for managing personal expenses. It allows users to add, view, edit, delete expenses, filter by date or category, view summaries with charts, and export to CSV. The backend uses Entity Framework Core with MySQL (hosted on XAMPP), and the frontend is Razor Views with Bootstrap for responsive UI. Developed in VS Code.
Setup Steps

Clone the Repository:
textgit clone https://github.com/yourusername/expense-tracker.git
cd expense-tracker

Install .NET SDK 8.0:

Download and install from [dotnet.microsoft.com/download/dotnet/8.0].


Install VS Code Extensions:

Open VS Code.
Install "C#" by Microsoft and "C# Dev Kit".


Set Up XAMPP:

Download and install XAMPP from [apachefriends.org].
Start Apache and MySQL in XAMPP Control Panel.
In phpMyAdmin (localhost/phpmyadmin), create a database named "expensesdb".


Configure Database Connection:

Open appsettings.json.
Update the connection string:
text"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=expensesdb;User=root;Password=;"
}



Apply Migrations:

Open terminal in VS Code.
Run:
textdotnet ef migrations add InitialCreate
dotnet ef database update



Run the Application:
textdotnet run

Open in browser: https://localhost:5001 or http://localhost:5000.
