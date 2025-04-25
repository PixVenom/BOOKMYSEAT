# 🎟️ BookMyShow Clone (Django)

A clone of the popular movie ticket booking platform [BookMyShow](https://in.bookmyshow.com/) built using **Django**. This project includes user authentication, movie listings, show timings, and booking functionalities.
---
## 🚀 Features

- 🔐 User authentication (signup/login/logout)
- 🎬 List of movies and detailed view
- 🕐 Show timings and booking system
- 🎟️ Ticket booking functionality
- 📁 Admin panel for managing content

---

## 🛠 Tech Stack

- Backend: **Django**
- Database: **PostgreSQL** (can use SQLite for local development)
- Frontend: **HTML, CSS, Bootstrap**
- Deployment: Designed for compatibility with **Render.com**

---

## 🔧 Setup Instructions

### 1. Clone the Repository

git clone https://github.com/BitHeadmr/djnago-bookmyshow-clone.git
cd djnago-bookmyshow-clone

# Create a virtual enviournment
python -m venv venv
source venv/bin/activate   # On Windows use: venv\\Scripts\\activate

# Install requirements
pip install -r requirements.txt

#Database setup
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}

python manage.py migrate

# Create a superuser
python manage.py createsuperuser

# Run the server
python manage.py runserver

#Folder Structure
bookmyshow_clone/
│
├── bookings/              # Booking logic & views
├── movies/                # Movie-related models & views
├── templates/             # HTML templates
├── static/                # CSS/JS
├── manage.py
└── requirements.txt
