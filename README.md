📚 Library_management_system
A Python-based Library Management System with MySQL integration and a Tkinter GUI. It efficiently supports book, user, and transaction management with real-time updates.

🚀 Features
🔐 Role-Based Access: Manage Admin, Librarian, and Student roles.
📚 Book Management: Add, search, delete, and view book details.
👥 User Management: Create, view, and remove user accounts.
🔄 Issue & Return Books: Track borrow and return activities with real-time stock updates.
📜 Transaction Records: Maintain complete issue/return history.
⏰ Fine Calculation Ready: Database includes a fine column for extensions.
🧾 Detailed Book Dialog: View complete book details and related transaction/user history.
🧠 Smart Refresh: Automatically updates all tables after changes.
🎨 Modern UI: Built with ttkthemes and PIL (Pillow) for themed design and background images.

💻 Technical Stack
Component	Technology
Programming Language	Python 3
GUI Framework	Tkinter, TTK Themes
Database	MySQL
Image Processing	Pillow (PIL)
IDE	Visual Studio Code

⚙️ Setup and Installation
1. Install Required Libraries
     Execute the following commands in your terminal to install the necessary Python dependencies:
       pip install mysql-connector-python
       pip install pillow
       pip install ttkthemes
2. Set up Database
You need to initialize the database schema and tables in MySQL.

Open your MySQL console, Workbench, or client.
Run the following SQL command to load the schema from the provided file:
SQL
SOURCE library_db.sql;
This script will create all three required tables:
  books
  users
  transactions

3. Update Connection Details
Before running the application, you must update the database credentials in the main file (lib.py).

Open the lib.py file.

Locate the mysql.connector.connect() function and modify the user and password parameters if they are different from the defaults:

Python

connection = mysql.connector.connect(
    host='localhost',
    user='root', # Ensure this is correct
    password='your_password', # Change this to your MySQL password!
    database='library_db'
)

▶️ Run the Project
Once the libraries are installed and the database credentials are set, run the application from your terminal:
python lib.py
