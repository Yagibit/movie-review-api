# movie-review-api

Movie Review Management API
This is a backend RESTful API built with Django and Django REST Framework. The project allows users to manage movie reviews by adding, updating, deleting, and viewing them through structured API endpoints.

  # Phase 3 Implementation Progress
As of this update, the following foundational tasks have been completed:

[x] Repository Setup: Initialized this GitHub repository for version control.

[x] Virtual Environment: Configured a Python venv to manage project dependencies.

[x] Project Initialization: Created the main Django project structure and the reviews application.

[x] Framework Configuration: Installed and configured Django REST Framework.


🛠️ Technology Stack

Backend Framework: Django 


API Framework: Django REST Framework 


Database: PostgreSQL (Production) / SQLite (Development) 


Authentication: Token-based 

📋 Database Architecture
The API is designed around three core entities:


User Table: Utilizes Django's built-in User model for authentication.


Movie Table: Stores film details including title, description, and release year.


Review Table: A bridge table linking users to movies, containing ratings (1-5) and review text.

📡 Planned API Endpoints

POST /api/users/register/ – Register a new user 


POST /api/users/login/ – Authenticate user 


GET /api/movies/ – List all movies 


POST /api/reviews/ – Create a review 


GET /api/movies/{id}/reviews/ – View reviews for a specific movie

# Phase 4 Implementation Progress

- User authentication using Django sessions
- CRUD operations for movies
- CRUD operations for reviews
- Only authenticated users can create, update, or delete reviews
- Users cannot modify or delete reviews created by others
- Validation for review ratings (1–5)
- Custom endpoint to view reviews for a specific movie
- Admin panel for managing users, movies, and reviews

