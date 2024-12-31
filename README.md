# Project_Name
Project Management API

# Description
This is a Django-based API for managing projects, including functionality to create, update, delete, and retrieve project data.

# Features
- Create, retrieve, update, and delete projects.
- Manage users and their associated roles.
- API endpoints for project and user management.

# Prerequisites
- Python 3.10 or later
- Django 4.x
- Git installed on your system

# Installation
1) Clone the repository:
'git clone https://github.com/mydhilimanoj/Project_Management.git'

2) Navigate to the project directory:
'cd Project_Management'

3) Create and activate a virtual environment
'python -m venv .venv
.venv\Scripts\activate
source .venv/bin/activate'

4) Install dependencies
'pip install -r requirements.txt'

5) Set up the database
'python manage.py makemigrations'
'python manage.py migrate'

6) Run the development server
'python manage.py runserver'

# API Documentation
The API documentation is generated using Swagger. It provides a user-friendly interface to explore and test the API endpoints
# Accessing Swagger Documentation
1) Run the development server
   python manage.py runserver
2) Open your browser and navigate to
   http://127.0.0.1:8000/swagger/
# Features of Swagger Documentation
- View all available API endpoints.
- Test API endpoints directly from the browser.
- Detailed information about request and response formats.

