📘 Python MySQL CRUD Application

This is a simple Command-Line CRUD (Create, Read, Update, Delete) application built using Python and MySQL. It allows users to manage records such as name, age, address, contact, and email.

🚀 Features

➕ Insert new records into MySQL database
📄 Display records in a formatted table
✏️ Update specific fields
❌ Delete records
🔄 Continuous menu-driven program
📊 Table display using tabulate

🛠️ Technologies Used

Python 3
MySQL Server
mysql-connector-python
tabulate

📦 Installation

1. Install Required Packages

pip install mysql-connector-python
pip install tabulate

2. Setup MySQL Database

Run the following SQL commands in MySQL:

CREATE DATABASE december_db;
USE december_db;
```
CREATE TABLE data (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    age INT,
    address VARCHAR(255),
    contact VARCHAR(15),
    mail VARCHAR(100)
);
```
⚙️ Configuration

Update your MySQL credentials in the script:
```
con = mysql.connector.connect(
    host="localhost",
    user="root",
    password="admin",
    database="december_db"
)
```
▶️ How to Run
python main.py

🧑‍💻 Usage

After running the program, you will see:
```
1.Insert Record
2.Select Record
3.Update Record
4.Delete Record
5.Exit
```
🔹 Insert Record

Add new user details

🔹 Select Record

Displays all records in table format

🔹 Update Record

Update specific fields using ID

🔹 Delete Record

Delete record by ID

📊 Sample Output
```
+----+--------+-----+-----------+-----------+------------------+
| ID | NAME   | AGE | ADDRESS   | CONTACT   | MAIL             |
+----+--------+-----+-----------+-----------+------------------+
| 1  | John   | 25  | Chennai   | 987654321 | john@email.com   |
+----+--------+-----+-----------+-----------+------------------+
```
⚠️ Notes

Ensure MySQL server is running
Use correct username and password
Table data must exist before running program
ID is auto-incremented

🔮 Future Improvements

Input validation
Search functionality
GUI interface (Tkinter / Web App)
Exception handling improvements
Export data to CSV/Excel

📜 License

This project is open-source and intended for educational purposes.