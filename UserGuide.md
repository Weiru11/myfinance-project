## UserGuide.md

### 👋 Welcome to MyFinance

This is a lightweight personal finance tracker designed for individual use. It allows you to log in, view your current balance, add income or expenses, and search records to manage your money.

---

### 🚪 Login

* Visit the login page (`login.php`)
* Enter any email and password
* The system accepts any input and grants access
* Once logged in, your session remains active until logout or browser close

---

### 📊 Main Dashboard (`myfinance.php`)

After logging in, you are directed to the main dashboard where you can:

* **Add a Transaction**

  * Enter the amount
  * Choose a category (e.g., Food, Transport)
  * Select a date and enter a description
  * Submit to save the transaction

* **View Summary**

  * The total balance is shown
  * A pie chart displays spending breakdown by category

* **View Records**

  * All transactions are listed in a table below the summary

---

### 🔍 Search Records (`keyword_search.php`)

* Navigate to the "Search Records" page from the navigation menu
* Enter a keyword (e.g., food, taxi)
* Optionally filter by category or date range
* Results will show all matching transactions

---

### 📅 Monthly Summary (`monthly_summary.php`)

* Navigate to the "Monthly Summary" page
* Select a month and year
* The page displays monthly totals and visual charts to summarize spending patterns

---

### 🚪 Logout

* Click the logout button in the top menu
* You will be returned to the login screen and session will end

---

### 🧪 Notes

* This system does not validate user accounts — login accepts any input
* All data is stored per session and managed in the database
* Intended for demonstration purposes

---

### 🛠 Tech Stack

* PHP (server-side scripting)
* MariaDB (database)
* HTML/CSS/JS (frontend)
* Apache (via XAMPP)
