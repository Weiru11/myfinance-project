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

#### 1. Download the Project from GitHub

* Visit the project repository (e.g., `https://github.com/your-username/myfinance`)
* Click the green **"Code"** button, then select **"Download ZIP"**
* Unzip the downloaded file
* Rename the extracted folder to `myfinance`

#### 2. Move Project to XAMPP

* Copy the entire `myfinance` folder to the `htdocs` directory of XAMPP:

  * Example: `C:/xampp/htdocs/myfinance`

#### 3. Start XAMPP Services

* Open the `XAMPP Control Panel`
* Start the following modules:

  * ✅ Apache
  * ✅ MySQL

#### 4. Create the Database

* Open your browser and go to `http://localhost/phpmyadmin`
* Click "New" on the left to create a new database:

  * Database name: `myfinance`
  * Collation: `utf8_general_ci`
* Import SQL file:

  * If the project includes `init.sql` , click "Import" and upload the file

#### 5. Configure Database Connection

* Open `config/database_config.php`
* Modify the settings as follows:
 <pre> ``` 
$host = 'localhost';
$dbname = 'myfinance';
$user = 'root';
$pass = ''; // Default XAMPP root has no password
```  </pre>
---

### ✅ Launch the Website

Open your browser and navigate to:

```
http://localhost/myfinance/
```

You should now see the login page.

---

### ❗ Troubleshooting

| Issue              | Solution                                                           |
| ------------------ | ------------------------------------------------------------------ |
| Apache won't start | Ensure no other programs are using ports 80/443 (e.g., Skype, IIS) |
| Login fails        | Not applicable — login accepts any input                           |
| Page not found     | Check that the folder name is `myfinance` and is inside `htdocs/`  |
| SQL import fails   | Make sure to select the correct database before importing SQL file |

If problems persist, check your database configuration in the `config/` folder or confirm that Apache and MySQL are both running in XAMPP.

