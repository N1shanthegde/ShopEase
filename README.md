# ShopEase Solution

ShopEase is a modern e-commerce solution built with ASP.NET Core (.NET 8), featuring a robust API backend and a user-friendly Razor Pages frontend.

---

## Projects Overview

### 1. WebApplication1 (API Backend)

- **Type:** ASP.NET Core Web API
- **Purpose:** Provides RESTful endpoints for products, orders, users, and authentication.
- **Key Features:**
  - Entity Framework Core with SQL Server support
  - JWT-based authentication and role-based authorization
  - AutoMapper for DTO/model mapping
  - Swagger/OpenAPI documentation
  - Identity integration for user management

### 2. WebApplication2 (Frontend)

- **Type:** ASP.NET Core Razor Pages
- **Purpose:** User-facing web application for shopping, order management, and account features.
- **Key Features:**
  - Razor Pages for dynamic, server-rendered UI
  - Product browsing, cart, and order management
  - Integration with backend API (WebApplication1)
  - Session-based authentication and JWT support
  - Responsive design with static assets in `wwwroot`
  - Client-side validation using jQuery Validation

---

## Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- Visual Studio 2022 or later
- SQL Server (or compatible database)

---

## Getting Started

### 1. Clone the Repository
### 2. Setup the API Backend (WebApplication1)
- Update the connection string in `appsettings.json` as needed.
- Apply database migrations:
- Run the API:
- The API will be available at `https://localhost:5001` (or as shown in the console).

### 3. Setup the Frontend (WebApplication2)

Open a new terminal:

- Update API endpoint URLs and settings in `appsettings.json` if needed.
- The frontend will be available at `https://localhost:5001` (or as shown in the console).

---

## Project Structure
ShopEase/
│
├── WebApplication1/        # Backend API
│   ├── Controllers/        # API controllers
│   ├── Models/             # Entity models
│   ├── DTOs/               # Data transfer objects
│   ├── Data/               # DbContext & migrations
│   └── appsettings.json    # Backend config
│
├── WebApplication2/        # Frontend Web App
│   ├── Pages/              # Razor Pages (.cshtml)
│   ├── Controllers/        # MVC controllers
│   ├── Dtos/               # DTOs for API communication
│   ├── wwwroot/            # Static files (CSS, JS, images)
│   └── appsettings.json    # Frontend config
│
└── README.md               # Documentation

---

## Acknowledgements

- Built with ASP.NET Core (.NET 8)
- Uses Entity Framework Core, AutoMapper, and Swashbuckle for API documentation
- Client-side validation powered by jQuery Validation


