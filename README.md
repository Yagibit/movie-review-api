# 🎬 Movie Review API

A RESTful Movie Review API built with **Django** and **Django REST Framework (DRF)**.  
This API allows users to create, view, update, delete, search, and filter movie reviews.  
Authentication and permissions ensure that only logged-in users can manage their own reviews.

The project is deployed live on **PythonAnywhere**.

---

## 🚀 Live Demo

Base URL:  
https://yagibit.pythonanywhere.com/api/

---

## 📌 Features

### 🔐 Authentication
- Uses Django’s built-in authentication system
- Only authenticated users can create, update, or delete reviews
- Users can only modify their **own** reviews

### 📝 Review Management (CRUD)
- Create a movie review
- View all reviews
- Update a review
- Delete a review

Each review includes:
- Movie Title
- Review Content
- Rating (1–5)
- User
- Created Date

### 🔍 Search, Filter & Sort
- Search reviews by **movie title**
- Filter reviews by **rating**
- Sort reviews by:
  - Rating
  - Date created
- Pagination for large datasets

---

## 🛠️ Tech Stack

- Python 3.10
- Django
- Django REST Framework
- SQLite (default)
- PythonAnywhere (deployment)

---

## 📂 Project Structure

```text
movie-review-api/
│
├── movie_api_project/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│
├── reviews/
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│
├── manage.py
├── requirements.txt
└── README.md

## 📡 API Endpoints

| Method | Endpoint               | Description                                            |
| ------ | ---------------------- | ------------------------------------------------------ |
| GET    | `/api/reviews/`        | List all reviews (supports search, filter, sort)       |
| POST   | `/api/reviews/`        | Create a new review (authenticated users only)         |
| GET    | `/api/reviews/{id}/`   | Retrieve a single review by ID                         |
| PUT    | `/api/reviews/{id}/`   | Fully update a review (owner & authenticated only)     |
| PATCH  | `/api/reviews/{id}/`   | Partially update a review (owner & authenticated only) |
| DELETE | `/api/reviews/{id}/`   | Delete a review (owner & authenticated only)           |
| GET    | `/api-auth/login/`     | Login (Browsable API)                                  |


## Validation Rules

Rating must be between 1 and 5

Movie title and review content are required

Unauthorized users cannot modify reviews

 ## Deployment

The project is deployed on PythonAnywhere using:

Manual web app configuration

WSGI setup

Virtual environment

Static files collection

## Author

Yared Getachew
Backend Developer – ALX Software Engineering Program