# pharmacy-management
Pharmacy management involves overseeing the operations of a pharmacy, including inventory control, staff supervision, and ensuring compliance with regulatory standards. It aims to provide efficient and safe medication distribution, optimize patient care, and maintain financial viability.

This project is a Pharmacy Management System built using Python's Tkinter for the GUI and MySQL for the database. The system allows users to manage medicine inventory, including adding, updating, deleting, and searching for medicines.

**Features**
Add Medicine: Insert new medicine details into the database.
Update Medicine: Modify existing medicine details in the database.
Delete Medicine: Remove a medicine entry from the database.
Search Medicine: Find medicines based on reference number, medicine name, or lot number.
Display Medicines: Show all medicines in the inventory.
**Prerequisites**
Python 3.x
Tkinter (usually included with Python installations)
MySQL
Installation
**Clone the repository**:

sh
Copy code
git clone https://github.com/your-username/pharmacy-management-system.git
cd pharmacy-management-system
Install MySQL:
Follow the instructions to install MySQL on your system from the official MySQL documentation.

Set up the database:

Open your MySQL command line or a MySQL client.
Create a new database named mydata:
sql
Copy code
CREATE DATABASE mydata;
USE mydata;
Create the pharmacy table:
sql
Copy code
CREATE TABLE pharmacy (
    REFRENCENO VARCHAR(50) PRIMARY KEY,
    MEDICINETYPE VARCHAR(50),
    MEDICINENAME VARCHAR(50),
    LOTNO VARCHAR(50),
    ISSUEDATE DATE,
    EXPDATE DATE,
    DOSAGE VARCHAR(50),
    PRICE DECIMAL(10, 2),
    PRODUCTQT INT
);
Configure database connection:

Update the connect_db function in your Python script if necessary:
python
Copy code
def connect_db():
    return sql.connect(host="localhost", user="your-username", password="your-password", database="mydata")
Install required Python packages:
Install the required packages using pip:

sh
Copy code
pip install mysql-connector-python
Usage
Run the Python script:

sh
Copy code
python pharmacy_management.py
The GUI window will open, allowing you to manage the pharmacy inventory through various functionalities like adding, updating, deleting, searching, and displaying medicines.

Code Overview
Database Connection:

python
Copy code
def connect_db():
    return sql.connect(host="localhost", user="root", password="riya123", database="mydata")
Fetch Data:
Fetch and display all medicine data from the database.

python
Copy code
def fetch_data():
    # code to fetch data from database
Insert Data:
Insert new medicine details into the database.

python
Copy code
def Insert():
    # code to insert data into database
Update Data:
Update existing medicine details in the database.

python
Copy code
def Update():
    # code to update data in database
Delete Data:
Delete a medicine entry from the database.

python
Copy code
def Del():
    # code to delete data from database
Search Data:
Search for medicines based on reference number, medicine name, or lot number.

python
Copy code
def search():
    # code to search data in database
Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue to improve the project.

**License**
This project is licensed under the MIT License. See the LICENSE file for more details.

Feel free to update the placeholders (e.g., GitHub repository URL, your username) and any other details as needed.










ChatGPT can make mistakes. Check
