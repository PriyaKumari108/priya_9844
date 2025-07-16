A Django-based Learning Management System (LMS) that provides RESTful APIs for user registration, user management, and course uploads. The system supports two user types: Teacher and Student.

Features
User signup with user type (Teacher/Student)
View all users
Update user email
Delete user by number
Upload and manage courses (for teachers)
SQLite database for development
Project Structure
PRIYA_LMS/
├── db.sqlite3
├── manage.py
├── PRIYA_COURSES/
│   ├── _init_.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── serlizers.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   └── migrations/
└── PRIYA_LMS/
    ├── _init_.py
    ├── asgi.py
    ├── settings.py
    ├── urls.py
    └── wsgi.py
Setup Instructions
Clone the repository:

git clone https://github.com/PriyaKumari108/priya_9844.git
cd PRIYA_LMS
Create a virtual environment and activate it:

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

pip install -r requirements.txt
Apply migrations:

python manage.py migrate
Run the development server:

python manage.py runserver
API Endpoints:

POST /signup/ - Register a new user
GET /getAllUsers/ - List all users
PUT /updateEmail/ - Update user email
DELETE /deleteUser/<number>/ - Delete user by number
