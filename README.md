# Inventory Management System

A web-based platform for managing inventory, purchases, and sales in retail or warehouse environments. This system enables efficient item tracking, customer/vendor management, and real-time stock updates — built with PHP and MySQL for simplicity and speed.

---

## Features

- User login system with roles (`admin`)
- Admin dashboard to manage:
  - Customers
  - Items
  - Vendors
  - Purchases
  - Sales
- Automatic stock updates on sale and purchase actions
- Responsive design using Bootstrap 
- Activity logging and real-time updates 

---

## Technologies Used

- **Frontend:** HTML, CSS, Bootstrap 
- **Backend:** PHP
- **Database:** MySQL
- **Server:** Apache (via XAMPP)

---

## Setup Instructions

### Clone the Repository
```bash
git clone https://github.com/yourusername/inventory-management-system.git
```

### Import the Database

1. Launch **phpMyAdmin** or MySQL CLI.
2. Create a new database named:
   ```
   shop_inventory
   ```
3. Import the SQL dump file:
   ```
   shop_inventory.sql
   ```

### Configure the App

1. Open the file:
   ```
   inc/config/constants.php
   ```
2. Set your site’s root URL and database credentials:
   ```php
   define("ROOT_URL", "http://localhost/inventory-management-system/");
   define("DB_HOST", "localhost");
   define("DB_USER", "root");
   define("DB_PASS", "");
   define("DB_NAME", "shop_inventory");
   ```

### Run Locally

1. Place the project folder inside your XAMPP `htdocs` directory.
2. Start **Apache** and **MySQL** via the XAMPP Control Panel.
3. In your browser, visit:
   ```
   http://localhost/inventory-management-system/login.php
   ```

---

## Login Credentials

- **Username:** `admin`
- **Password:** `admin`

---

## Folder Structure (Key Files)

| File / Folder              | Description                                 |
|---------------------------|---------------------------------------------|
| `login.php`               | Login interface for users                   |
| `user.php`                | User account logic                          |
| `customer.php`            | Customer management (CRUD)                  |
| `item.php`                | Inventory item management                   |
| `purchase.php`            | Purchase logging and stock updates          |
| `sale.php`                | Sales management and stock deduction        |
| `vendor.php`              | Vendor management                           |
| `inc/config/constants.php`| Configuration settings and DB credentials   |
| `shop_inventory.sql`      | SQL dump for database structure and data    |

---

## Authors

- ZARA KHALID  
- ZAIB SAADAT

---

## License

This project is intended for educational purposes only.

---

> 🛡️ Stay organized. Stay efficient.
