⚙️ How to Configure the Application

1. Database Configuration

Navigate to /config/

Copy database_config.template.php and rename it as database_config.php

Edit database_config.php to match your environment:

define('DB_HOST', 'localhost');
define('DB_NAME', 'myfinance');
define('DB_USER', 'root');
define('DB_PASS', ''); // Default for XAMPP

2. Set Up the Database

Open a browser and visit: http://localhost/phpmyadmin

Create a new database named myfinance

Option A: Import schema.sql if provided

Option B: Visit http://localhost/myfinance/page_php/setup_database.php to auto-generate tables

3. Configure Session Behavior (Optional)

Edit config/app.php to set session lifetime and timeout

Make sure each protected page starts with:

session_start();
if (!isset($_SESSION['user_id'])) {
    header("Location: login.php");
    exit;
}

🧹 How to Maintain the Application

1. Backing Up Data

Use phpMyAdmin to export the database regularly:

Select myfinance database

Click "Export" > Format: SQL > Go

Optionally automate export using cron jobs or scripts if on Linux

2. Resetting Transactions

Use SQL to truncate tables (e.g., transactions, categories) if needed:

TRUNCATE TABLE transactions;
TRUNCATE TABLE categories;

3. Adding or Editing Categories

Categories are stored in the categories table

Use phpMyAdmin or create/edit via admin-only interface if implemented

4. Monitoring Server Logs

Apache logs (errors): C:/xampp/apache/logs/error.log

PHP errors: Enable display_errors in php.ini during development only

5. Updating the Application

Pull from GitHub if version-controlled

Overwrite project folder except for /config/database_config.php

Re-check database schema compatibility before applying changes

👨‍🔧 Admin Access

This system does not include a formal admin login panel

Admin access and maintenance are expected to be handled directly via filesystem and database tools like phpMyAdmin

