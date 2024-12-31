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

# Setup Swagger
1) Install the required package :
   pip install drf-yasg

2) Add the following to urls.py
from django.urls import path
from rest_framework import permissions
from drf_yasg.views import get_schema_view
from drf_yasg import openapi

schema_view = get_schema_view(
    openapi.Info(
        title="Project Management API",
        default_version="v1",
        description="API documentation for the Project Management system",
        terms_of_service="https://www.google.com/policies/terms/",
        contact=openapi.Contact(email="your_email@example.com"),
        license=openapi.License(name="MIT License"),
    ),
    public=True,
    permission_classes=(permissions.AllowAny,),
)

urlpatterns = [
    # Other paths
    path("swagger/", schema_view.with_ui("swagger", cache_timeout=0), name="schema-swagger-ui"),
]

3) Run the server and access the Swagger documentation at /swagger/

