# MyFinance

A lightweight web-based finance tracker built with PHP and MariaDB. This project allows users to log in (without authentication), manage simple income/expense entries, search through past transactions, and track their balance in a dashboard interface.

---

## 🔧 Features

* Simple login with any credentials (no user verification)
* Add, view, and manage income or expense records
* Search records by keyword (e.g., description or category)
* Summary balance display
* Minimal, clean frontend using HTML/CSS/JS
* Easy deployment with XAMPP

---

## 📁 Project Structure

```
myfinance-project/
├── config/             # PHP configuration files (database, security)
├── css/                # Stylesheets
├── js/                 # JavaScript files
├── pages/              # HTML pages (login, myfinance)
├── page_php/           # PHP backend logic (login_process, data handling)
├── database/           # SQL files for schema or demo data
├── index.php           # Main entry point
```

---

## 🚀 Installation

See `Installation.md` for full setup instructions using XAMPP.

---

## 🧭 Usage Guide

See `UserGuide.md` for details on login behavior, dashboard functions, and how to interact with the system.

---

## ⚠️ Disclaimer

This system is for demonstration purposes only:

* No password authentication or encryption is implemented
* All users share the same access
* Not suitable for production use without security enhancements

---

## 👩‍💻 Tech Stack

* PHP (Server-side)
* MariaDB (Database)
* HTML, CSS, JavaScript
* XAMPP (Apache + MySQL)
