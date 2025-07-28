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

## 📁 Folder Structure

Sanayii_Admin-Dashboard/
│
├── Controllers/ → MVC controllers (e.g., UserController, ArtisanController)
├── Models/ → Domain models (e.g., User, Artisan, ServiceRequest)
├── ViewModels/ → View models used in forms and UI
├── Views/ → Razor views (.cshtml files)
│ ├── Shared/ → Layout and partial views
│ └── Dashboard/ → Main admin screens
│
├── Data/ → ApplicationDbContext and DB initializer
├── Migrations/ → EF Core migrations
├── Services/ → Business logic and helper services
├── wwwroot/ → Static assets (CSS, JS, Images)
├── appsettings.json → App configuration
└── Program.cs / Startup.cs → App entry point and middleware setup

yaml
Copy
Edit

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
⚙️ 2. Configure the Database
In appsettings.json, update your database connection string:

json
Copy
Edit
"ConnectionStrings": {
  "DefaultConnection": "Server=.;Database=SanayiiDB;Trusted_Connection=True;"
}
🧱 3. Apply Migrations
bash
Copy
Edit
dotnet ef database update
Or use Visual Studio's Package Manager Console.

▶️ 4. Run the Application
bash
Copy
Edit
dotnet run
Then navigate to:
👉 https://localhost:5001 or http://localhost:5000

🔐 Admin Login
Use the default seeded admin account:

text
Copy
Edit
Email: admin@sanayii.com
Password: Admin@123
Or create a user and assign the admin role manually in the database.

✅ Features
JWT + Refresh token authentication (if integrated)

Role-based access (Admin / Viewer)

Manage users and artisans

Approve or reject artisan applications

Monitor service requests and history

Responsive Bootstrap UI

Chat/message log monitoring (if SignalR connected)

Dashboard analytics (optional)

🧪 Testing
(Coming Soon) Unit testing with xUnit and Moq

📄 License
This project is licensed under the MIT License.

👩‍💻 Author
Aya Mohamed Nafed

📬 Contact
For questions, feedback, or contributions, feel free to open an issue or reach  out via LinkedIn.
