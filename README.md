# MySQL CRUD Console Application

A Python console application that performs CRUD (Create, Read, Update, Delete) operations on a MySQL database with a user-friendly interface.

## Features
- 🆕 Create new records with full details
- 👀 View all records in formatted tables
- ✏️ Update specific fields (name, age, address, contact, or email)
- ❌ Delete records by ID
- 🔄 Interactive console menu
- 📊 Tabular data display using `tabulate`

## Prerequisites
- Python 3.6+
- MySQL Server
- MySQL Connector/Python
- Tabulate package

## Installation
```bash
# Clone the repository
git clone https://github.com/dineshkumar-account/MySQL-CONNECTOR-CRUD-Application.git

# Install dependencies
pip install mysql-connector-python tabulate
Database Setup
Create a MySQL database (or use existing one)

Create the required table:

sql
CREATE TABLE data (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    age INT,
    address VARCHAR(255),
    contact VARCHAR(20),
    mail VARCHAR(100)
);
Configuration
Edit the connection parameters in the script:

python
con = mysql.connector.connect(
    host="localhost",  # Your MySQL host
    user="root",       # Your MySQL username
    password="",       # Your MySQL password
    database=""        # Your database name
)
Usage
Run the application:

bash
python crud_app.py
Menu Options:
Insert Record - Add new person with all details

Select Record - View all records in formatted table

Update Record - Modify specific fields:

Name

Age

Address

Contact

Email

Delete Record - Remove record by ID

Exit - Close the application

Screenshot
text
1. Insert Record
2. Select Record
3. Update Record
4. Delete Record
5. Exit

Enter Your Choice : 2

ID    NAME       AGE    ADDRESS          CONTACT       MAIL
----  ---------  -----  ---------------  ------------  ------------------
1     John Doe   28     123 Main St      +1234567890   john@example.com
2     Jane Smith 32     456 Oak Avenue   +9876543210   jane@example.com
Requirements
Create requirements.txt with:

text
mysql-connector-python==8.1.0
tabulate==0.9.0
Project Structure
text
mysql-crud-app/
├── crud_app.py        # Main application file
├── README.md          # Documentation
└── requirements.txt   # Dependencies
License
MIT License - Free to use and modify

text

Key features of this README:
1. Clear visual hierarchy with emojis
2. Complete setup instructions
3. Database schema included
4. Screenshot of expected output
5. Menu options explained
6. Simple requirements specification