# Backend-Capstone

This project is the Little Lemon Restaurant API, developed using the Django REST Framework.
It demonstrates the ability to build a backend service that connects to a MySQL database, supports user authentication, and exposes RESTful API endpoints.

Project Overview

The backend manages menu items and table bookings.
The application also includes user registration and authentication, so that customers and staff can securely interact with the system.

The API can handle standard HTTP requests:

GET – retrieve menu items or bookings

POST – create new items or bookings

PUT – update existing records

DELETE – remove items or bookings

API Endpoints to Test

Menu API

/api/menu/ → View all menu items or add a new one

/api/menu/<id>/ → View, update, or delete a specific menu item

Bookings API

/api/bookings/ → View all bookings or add a new booking

/api/bookings/<id>/ → View, update, or delete a booking

User Registration and Authentication

/api/registration/ → Create a new user account

/api/token/ → Obtain a JWT authentication token

/api/token/refresh/ → Refresh the JWT token

Database

The backend uses a MySQL database to store menu and booking information.
Django models are mapped to database tables, ensuring smooth data management and consistency.

Testing Instructions

Clone the GitHub repository containing this project.

Install dependencies listed in requirements.txt.

Apply migrations and run the server with python manage.py runserver.

Use Insomnia or Postman to test the API paths listed above.

Authentication endpoints should be tested first to obtain a token before accessing protected routes.

Unit Tests

Basic unit tests are included to validate:

API responses

CRUD operations

Authentication flow
