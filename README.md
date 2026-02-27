# 📝 CLI Notes App (Python)

A simple command-line based Notes Management System built with Python.
It supports user authentication, note creation, search, and deletion, with file-based storage and basic logging.

This project demonstrates OOP design, input validation, file handling, and modular architecture in Python.

# 🚀 Features

🔐 User Registration & Login

📝 Add Notes with auto-generated IDs & timestamps

📖 View all notes

🔍 Search notes by keyword

🗑️ Delete notes by ID

📂 File-based storage per user

⚠️ Error logging system

✅ Input validation for users and notes

# 🏗️ Project Structure
notes_app.py
users.txt              # Stores registered users (auto-created)
<username>_notes.txt   # Notes file per user (auto-created)
error.log              # Application error logs

# 🧠 Architecture

The application follows an object-oriented design:

Class	Responsibility

Note	Represents a single note with ID, content, timestamp

User	Stores user credentials and note file mapping

Validator	Validates usernames, passwords, note content, and IDs

FileManager	Handles file read/write/append operations

AuthManager	Manages user registration and login

NotesManager	Handles note CRUD operations and search

Logger	Logs errors and info messages to error.log

NotesApp	Main CLI controller and menu navigation

# ⚙️ Requirements

Python 3.8+

No external dependencies (uses only Python standard library)

# ▶️ How to Run
python notes_app.py

# 🖥️ Usage Flow
1️⃣ Start Menu
1. Register
2. Login
3. Exit
2️⃣ After Login
1. Add Note
2. View Notes
3. Delete Note
4. Search Notes
5. Logout

# 📄 Example Note Format
ID: 1
Time: 2026-02-27 10:30:15.123456
Content: Finish GitHub README
------------------------------
# 🔐 Data Storage

User credentials are stored in:

users.txt

Each user gets a separate notes file:

<username>_notes.txt

# ⚠️ Passwords are stored in plain text (for learning purposes only).

Do not use this approach in production.

# 🪵 Logging

All unexpected errors are recorded in:
error.log

# ⚠️ Known Issues / Limitations

Passwords are not hashed (security improvement needed)

Notes are stored as plain text instead of structured format (e.g., JSON/DB)

No pagination for large note sets

Minor typo bug in delete_note():

notes_in.strop()

should be:
notes_in.strip()

# 🔮 Future Enhancements

🔒 Password hashing (bcrypt)

🗃️ SQLite or PostgreSQL integration

🖥️ GUI version (Tkinter / PyQt)

🌐 REST API (Flask/FastAPI)

🏷️ Note tagging & categories

📅 Date-based filtering

📤 Export notes to Markdown/PDF


# 🧪 Learning Outcomes

This project helps practice:

Object-Oriented Programming (OOP)

File handling in Python

CLI application design

Input validation

Separation of concerns

Basic authentication logic

Logging and error handling

# 🤝 Contributing

Contributions are welcome!
Fork the repo
Create a feature branch
Commit your changes
Open a Pull Request

# 📜 License

This project is licensed under the MIT License.

# 👩‍💻 Author

Sangita Bera

Python Developer | Backend Enthusiast
