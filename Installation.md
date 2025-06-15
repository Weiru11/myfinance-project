## Installation.md

### 📦 Installation & Launch Instructions

This document provides step-by-step instructions to install and run the MyFinance web application on a local environment.

---

### 🖥️ System Requirements

* Operating System: Windows 10 or later
* Software:

  * [XAMPP](https://www.apachefriends.org/index.html) (includes Apache, MariaDB, PHP)
  * Web browser (e.g., Chrome, Firefox)

---

### 🚀 Installation Steps

#### 1. Install XAMPP

* Visit the [XAMPP website](https://www.apachefriends.org/index.html) and download the Windows version.
* Run the installer and select Apache and MySQL (default options).
* After installation, open the `XAMPP Control Panel` and start:

  * ✅ Apache
  * ✅ MySQL

#### 2. Place Project Files

* Unzip the file `finance-2-fixed.zip`
* Rename the extracted folder to `myfinance`
* Copy the entire folder to the `htdocs` directory in XAMPP:

  * Example: `C:/xampp/htdocs/myfinance`

#### 3. Create Database

* Open your browser and go to `http://localhost/phpmyadmin`
* Click "New" on the left to create a new database:

  * Database name: `myfinance`
  * Collation: `utf8_general_ci`
* Import SQL file: If the project includes `myfinance.sql` or `schema.sql`, click "Import" and upload the file.

#### 4. Configure Database Connection

* Open `config/database.php` or `config/database_config.php`
* Modify the settings as follows:

```php
$host = 'localhost';
$dbname = 'myfinance';
$user = 'root';
$pass = ''; // Default XAMPP root has no password
```

---

### ✅ Launch the Website

Open your browser and navigate to:

```
http://localhost/myfinance/
```

You should now see the login page. Enter any email and password to access the dashboard.

---

### ❗ Troubleshooting

| Issue              | Solution                                                           |
| ------------------ | ------------------------------------------------------------------ |
| Apache won't start | Ensure no other programs are using ports 80/443 (e.g., Skype, IIS) |
| Login fails        | Not applicable — login accepts any input                           |
| Page not found     | Check that the folder name is `myfinance` and is inside `htdocs/`  |
| SQL import fails   | Make sure to select the correct database before importing SQL file |

If problems persist, check your database configuration in the `config/` folder or confirm that Apache and MySQL are both running in XAMPP.
