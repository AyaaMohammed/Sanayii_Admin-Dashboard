# Sanayii Admin Dashboard (ASP.NET Core MVC)

🔧 **Sanayii_Admin-Dashboard**  
A smart admin dashboard for managing the Sanayii Platform — a system that connects clients with certified artisans using real-time communication, intelligent matchmaking, and secure contract handling.

---

## 📌 Overview

The admin dashboard allows administrators to:

- ✅ Manage users and artisans  
- 🔍 Review service requests and platform activity  
- 🧾 Approve or reject artisan applications  
- 💬 Monitor communication and chat logs  
- 🔐 Control access, roles, and permissions  

Built using **ASP.NET Core MVC** following **Clean Architecture principles**.

---

## 🧰 Tech Stack

- ASP.NET Core MVC (.NET 7 / .NET 8)  
- Entity Framework Core  
- SQL Server  
- ASP.NET Identity (with Role Management)  
- AutoMapper  
- Bootstrap 5  
- LINQ / TempData / ViewModels  

---

## 🚀 Getting Started

### ✅ Prerequisites

- .NET SDK 7 or 8  
- SQL Server or LocalDB  
- Visual Studio 2022+ or VS Code  

---

### 📦 1. Clone the Repository

```bash
git clone https://github.com/AyaaMohammed/Sanayii_Admin-Dashboard.git
cd Sanayii_Admin-Dashboard
```

---

### ⚙️ 2. Configure the Database

In `appsettings.json`, update your database connection string.

---

## 🔗 Database Connection String & AppSettings

Open `appsettings.json` and modify your connection string and basic settings as follows:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=.;Database=SanayiiDB;Trusted_Connection=True;"
  },
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Warning"
    }
  },
  "AllowedHosts": "*"
}
```

- Replace `Server=.;` with your actual SQL Server name if needed.  
- You can also use SQL Authentication like this:

```json
"DefaultConnection": "Server=localhost;Database=SanayiiDB;User Id=your_username;Password=your_password;"
```

---

### 🧱 3. Apply Migrations

```bash
dotnet ef database update
```

Or use Visual Studio's Package Manager Console.

---

### ▶️ 4. Run the Application

```bash
dotnet run
```

Then navigate to:  
👉 https://localhost:5001 or http://localhost:5000

---

🔐 **Admin Login**

Use the default seeded admin account:

```
Email: admin@sanayii.com  
Password: Admin@123
```

Or create a user and assign the admin role manually in the database.

---

## ✅ Features

- JWT + Refresh token authentication (if integrated)  
- Role-based access (Admin / Viewer)  
- Manage users and artisans  
- Approve or reject artisan applications  
- Monitor service requests and history  
- Responsive Bootstrap UI  
- Chat/message log monitoring (if SignalR connected)  
- Dashboard analytics (optional)  

---

## 🧪 Testing

(Coming Soon) Unit testing with xUnit and Moq

---

## 📄 License

This project is licensed under the MIT License.

---

## 👩‍💻 Author

**Aya Nafed**

---

## 📬 Contact

For questions, feedback, or contributions, feel free to open an issue or reach out via LinkedIn.
