# Online Bookstore Project (OBS Project)

A full-featured **Online Bookstore** built with **Django**. This project includes both **Admin** and **User** dashboards, enabling book management, order tracking, user management, and seamless payment via **Stripe**.

---

📁 Folder Structure

```
obsproject/
│
├── manage.py
├── db.sqlite3
├── .gitignore
├── .env
│
├── obsproject/ # Main project configuration folder
│ ├── init.py
│ ├── asgi.py
│ ├── settings.py # Global Django settings
│ ├── urls.py # Root URL configuration
│ ├── wsgi.py
│ └── pycache/
│
├── adminapp/ # Admin-side application
│ ├── init.py
│ ├── admin.py
│ ├── adminappurls.py # Admin app specific URLs
│ ├── apps.py
│ ├── models.py
│ ├── tests.py
│ ├── views.py
│ ├── migrations/
│ ├── static/ # Admin-specific static files (CSS, JS, Images)
│ └── templates/ # Admin HTML templates
│
├── userapp/ # User-side application
│ ├── init.py
│ ├── admin.py
│ ├── userappurls.py # User app specific URLs
│ ├── apps.py
│ ├── models.py
│ ├── tests.py
│ ├── views.py
│ ├── migrations/
│ ├── static/ # User static files
│ └── templates/ # User HTML templates
│
└── myapp/ # Common/shared application
├── init.py
├── admin.py
├── apps.py
├── models.py
├── myapp_urls.py # Common/shared URLs
├── tests.py
├── views.py
├── migrations/
├── static/ # Common static assets
└── templates/ # Common templates


⚙️ Features    

### Admin Dashboard
- Add, update, rename, and delete **book categories** and **book details**.
- Manage **orders** and view **order history**.
- Complete control over the bookstore inventory.

### User Dashboard
- **View and edit profile** information.
- **Change password** securely.
- Browse and **buy books**.
- **Stripe payment gateway integration** for safe and smooth transactions.
- View order history.

### Common Features
- Responsive design for desktop and mobile.
- Shared templates and static files for consistency.
- Modular Django app structure for scalability.

---

## 💻 Technologies Used
- **Backend:** Python, Django  
- **Frontend:** HTML, CSS, JavaScript, Bootstrap (optional)  
- **Database:** SQLite  
- **Payment Integration:** Stripe  

---




```
🚀 Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/Archer1200/Online_book_store.git
cd obsproject
```
2. **Create virtual environment**
```
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows
```

3. **Install dependencies**
```
pip install -r requirements.txt
```

4. **Configure environment variables**

Rename .env.example to .env and add your Stripe API keys and Django secret key.
```
Run migrations
python manage.py makemigrations
python manage.py migrate
```

5. **Create superuser**

```
python manage.py createsuperuser
```

5. **Start the development server**
```
python manage.py runserver
```

Visit http://127.0.0.1:8000/ to access the application.





