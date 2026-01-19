# .NET


# 📦 Product Inventory Management API

An **ASP.NET Core Web API** for managing product inventory using **Entity Framework Core**.
This project is designed as an **academic / practical project** to demonstrate CRUD operations, RESTful APIs, and database integration in .NET.

---

## 📌 Project Title

**Product Inventory Management API**

---

## 🧾 Problem Statement

Develop an ASP.NET Core Web API to manage product inventory. The API should allow users to add, view, update, and delete product records stored in a database using Entity Framework Core.

---

## 🚀 Features

* Create new products
* View all products
* View product by ID
* Update product details
* Delete product records
* Uses **Entity Framework Core** with **Code First approach**
* RESTful API design

---

## 🛠️ Technology Stack

* ASP.NET Core Web API
* C#
* Entity Framework Core
* SQL Server (LocalDB / SQL Server)
* Swagger (OpenAPI)

---

## 📂 Project Structure

```
ProductInventoryAPI/
│
├── Controllers/
│   └── ProductController.cs
│
├── Data/
│   └── ApplicationDbContext.cs
│
├── Models/
│   └── Product.cs
│
├── Migrations/
│
├── Program.cs
├── appsettings.json
└── README.md
```

---

## 📦 Product Entity

The **Product** entity contains the following fields:

* **Id** (GUID)
* **ProductName**
* **Category**
* **Price**
* **StockQuantity**

---

## 🔗 API Endpoints

### 📍 Get All Products

```
GET /api/product
```

### 📍 Get Product by ID

```
GET /api/product/{id}
```

### 📍 Add a New Product

```
POST /api/product
```

### 📍 Update Product Details

```
PUT /api/product/{id}
```

### 📍 Delete a Product

```
DELETE /api/product/{id}
```

---

## ⚙️ Database Configuration

The project uses **ApplicationDbContext** with **DbSet<Product>**.

Connection string is configured in **appsettings.json**.

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=ProductInventoryDB;Trusted_Connection=True;"
}
```

---

## ▶️ How to Run the Project

### Prerequisites

* .NET SDK 6 / 7 / 8
* SQL Server or LocalDB
* Visual Studio 2022

### Steps

1. Clone the repository
2. Open the project in Visual Studio
3. Update the database connection string if required
4. Run the following commands in **Package Manager Console**:

```
Add-Migration InitialCreate
Update-Database
```

5. Press **Run** ▶️
6. Swagger UI will open automatically

---

## 🧪 Testing the API

* Use **Swagger UI** (default)
* Or test using **Postman**

---

## 🎯 Learning Outcomes

* Understanding ASP.NET Core Web API
* Implementing CRUD operations
* Working with Entity Framework Core
* REST API development
* Database integration

---

