# Django Blog Project

## Overview

This is a full-featured Django Blog Application built as a real-world project to demonstrate production-level web development using Django.

The project includes blog management, authentication, role-based dashboards, comments, search functionality, and media handling with a scalable database setup.

It is designed with clean architecture, modular apps, and deployment readiness in mind.

---

## What This Project Demonstrates

- Django project structuring (real-world architecture)
- Blog CRUD operations (Create, Read, Update, Delete)
- User authentication system (login, logout, registration)
- Role-based access control (Admin / Author / Staff logic)
- PostgreSQL database integration
- Image upload and media handling
- Dashboard system for managing content
- Search and filtering functionality
- Template inheritance and reusable UI components
- Production-ready deployment configuration

---

## Features

### Blog System
- Create and manage blog posts
- Featured images for posts
- Slug-based URLs
- Category-based organization
- Featured posts support

### User System
- User registration and login
- Secure authentication using Django auth
- Role-based permissions system

### Comments System
- Authenticated user comments
- Comment timestamps
- Comment count display

### Search System
- Search blogs by title and content
- Persistent search input

### Dashboard
- Custom admin dashboard
- Blog and category management
- User-based content control

---

## Database

- PostgreSQL used for production-level database management

---

## Tech Stack

- **Backend:** Django 6
- **Frontend:** HTML, CSS, Bootstrap
- **Database:** PostgreSQL
- **Authentication:** Django built-in auth system
- **Environment Management:** python-dotenv

---

## Project Structure

```bash
blog_main/
│
├── blogs/              # Blog application
├── dashboard/          # Dashboard system
├── core/               # Core utilities and views
├── templates/          # HTML templates
├── static/             # Static assets
├── media/              # Uploaded files (development)
├── blog_main/          # Project settings

```

Installation & Setup
1. Clone repository
git clone https://github.com/your-username/django-blog.git
cd django-blog
2. Create virtual environment
python -m venv env
env\Scripts\activate   # Windows
3. Install dependencies
pip install -r requirements.txt
4. Configure .env
SECRET_KEY=your_secret_key
DEBUG=True

DB_NAME=your_db
DB_USER=postgres
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=5432
5. Run migrations
python manage.py makemigrations
python manage.py migrate
6. Create superuser
python manage.py createsuperuser
7. Run server
python manage.py runserver