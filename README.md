# LIbrary_management_system
A Python-based Library Management System with MySQL integration and a Tkinter GUI — supports book, user, and transaction management with real-time updates.

🚀 Features

🔐 Role-Based Access: Manage Admin, Librarian, and Student roles
📚 Book Management: Add, search, delete, and view book details
👥 User Management: Create, view, and remove user accounts
🔄 Issue & Return Books: Track borrow and return activities with real-time stock updates
📜 Transaction Records: Maintain complete issue/return history
⏰ Fine Calculation Ready: Database includes a fine column for extensions
🧾 Detailed Book Dialog: View complete book details and related transaction/user history
🧠 Smart Refresh: Automatically updates all tables after changes
🎨 Modern UI: Built with ttkthemes and PIL for themed design and background images


1.| Component            | Technology          |
  | -------------------- | ------------------- |
  | Programming Language | Python 3            |
  | GUI Framework        | Tkinter, TTK Themes |
  | Database             | MySQL               |
  | Image Processing     | Pillow (PIL)        |
  | IDE                  | Visual Studio Code  |

2. Install Required Libraries:-
   pip install mysql-connector-python
   pip install pillow
   pip install ttkthemes

3. Set up Database:-
   Open MySQL and run:
   SOURCE library_db.sql;

   This will create all tables:-
     •books
     •users
     •transactions

4. Update Connection Details:-
In lib.py, modify your database credentials (if needed):
connection = mysql.connector.connect(
    host='localhost',
    user='root',
    password='your_password',
    database='library_db'
)

5. python lib.py
