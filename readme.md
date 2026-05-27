# Django Custom User Authentication System

A Django REST Framework based authentication system using a custom user model with email authentication, token authentication, password management, and REST APIs.

---

# Project Overview

This project provides a complete authentication and user management system using:

- Django
- Django REST Framework (DRF)
- Token Authentication
- Custom User Model
- Email-based Login
- REST APIs

The system supports both template-based authentication and REST API authentication.

---

# Features

## Authentication Features

- User Registration
- User Login
- User Logout
- Change Password
- Token Authentication
- Email Authentication
- Custom User Model

---

## User Management Features

- Custom User Fields
- User List API
- Admin Panel Support
- Password Encryption
- Form Validation
- API Validation

---

# Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend Programming |
| Django | Web Framework |
| Django REST Framework | REST APIs |
| SQLite / PostgreSQL | Database |
| Token Authentication | API Security |
| HTML/CSS | Frontend Templates |

---

# Custom User Model

The project uses a fully customized Django user model.

## User Fields

| Field Name | Type |
|---|---|
| email | EmailField |
| Full_Name | CharField |
| Gender | CharField |
| Marital_Status | CharField |
| Mother_Tongue | CharField |
| Mobile_No | CharField |

---

# API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | /api/register/ | Register New User |
| POST | /api/login/ | User Login |
| POST | /api/logout/ | User Logout |
| GET | /api/users/ | Get User List |
| PUT | /api/change-password/ | Change Password |

---

# Authentication Flow

## Registration

1. User submits registration form
2. Password validation performed
3. Password encrypted using Django hashing
4. User account created

---

## Login

1. User submits email and password
2. Credentials validated
3. Authentication token generated
4. Token returned to client

---

## Protected APIs

Protected APIs require:

```bash
Authorization: Token your_token_here
```

---

# Installation

## Clone Project

```bash
git clone project_url
```

---

## Create Virtual Environment

```bash
python -m venv env
```

---

## Activate Environment

### Windows

```bash
env\Scripts\activate
```

### Linux / Mac

```bash
source env/bin/activate
```

---

# Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Database Migration

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

---

# Create Superuser

```bash
python manage.py createsuperuser
```

---

# Run Development Server

```bash
python manage.py runserver
```

---

# Sample API Request

## Registration

```json
{
    "email": "test@gmail.com",
    "Full_Name": "Manikandan",
    "Gender": "Male",
    "Marital_Status": "Single",
    "Mother_Tongue": "Tamil",
    "Mobile_No": "9876543210",
    "password1": "Admin@123",
    "password2": "Admin@123"
}
```

---

# Sample Login Request

```json
{
    "email": "test@gmail.com",
    "password": "Admin@123"
}
```

---

# Security Features

- Password Hashing
- Token Authentication
- Password Validation
- Protected APIs
- Authenticated Endpoints
- Django Authentication System

---

# Future Improvements

- JWT Authentication
- Email Verification
- Forgot Password
- OTP Verification
- User Profile Upload
- Role Based Authentication
- Social Login
- Swagger Documentation

---

# Admin Panel

Django admin panel supports:

- User Management
- Permission Management
- Staff Management
- Superuser Access

---

# Project Structure

```bash
project/
│
├── users/
│   ├── admin.py
│   ├── forms.py
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│
├── templates/
│
├── manage.py
│
├── requirements.txt
│
└── settings.py
```

---

# Author

## Developer

Manikandan R

---

# License

This project is developed for learning and development purposes.