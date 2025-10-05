# 🚀 SaaSify — Modern Django SaaS Web App

SaaSify is a **modern SaaS starter web application** built with **Django, Tailwind CSS, and SQLite**.  
It includes **authentication, user profile management, contact form, and dashboard UI** — designed for speed, scalability, and a professional look.

---

## 📖 Table of Contents
- [✨ Overview](#-overview)
- [🎯 Features](#-features)
- [🧠 Project Structure](#-project-structure)
- [🛠️ Tech Stack](#️-tech-stack)
- [⚙️ Installation & Setup](#️-installation--setup)
- [🔐 Authentication Flow](#-authentication-flow)
- [👤 User Profile Management](#-user-profile-management)
- [💬 Contact Form](#-contact-form)
- [📂 Static Files](#-static-files)
- [🚀 Deployment Ready](#-deployment-ready)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Overview

**SaaSify** is a ready-to-use Django boilerplate that comes with:
- Authentication (Login / Signup / Logout)
- User Profile Management with Edit functionality
- Tailwind UI design with responsive layouts
- Contact Form with message saving
- Dashboard-like Profile Analytics

You can use SaaSify as a **foundation** for SaaS products, dashboards, or internal tools.

---

## 🎯 Features

✅ User Registration & Login  
✅ Secure Authentication using Django Auth  
✅ Profile Page with Update (Name, Email)  
✅ Contact Form with Database Integration  
✅ Tailwind CSS UI  
✅ Flash Messages for Success/Error  
✅ Protected Routes using `@login_required`  
✅ Clean URL Routing  
✅ Modular App Structure (`accounts`, `pages`)  
✅ Ready for Production Deployment

---

## 🧠 Project Structure

saasify/
│
├── accounts/ # Authentication & Profile Management
│ ├── templates/accounts/ # login.html, register.html, profile.html
│ ├── forms.py
│ ├── models.py
│ ├── urls.py
│ └── views.py
│
├── pages/ # Static pages (Home, About, Contact)
│ ├── templates/pages/
│ ├── forms.py
│ ├── models.py
│ ├── urls.py
│ └── views.py
│
├── static/ # Static assets
│ ├── css/
│ └── images/
│
├── templates/ # Base templates
│ ├── base.html
│
├── saasify/ # Project root config
│ ├── urls.py
│ └── settings.py
│
├── manage.py
└── README.md

yaml
Copy code

---

## 🛠️ Tech Stack

| Category | Technology |
|-----------|-------------|
| Framework | **Django 5+** |
| Frontend  | **Tailwind CSS** |
| Database  | **SQLite** (default) |
| Auth      | **Django Auth System** |
| UI Icons  | **Heroicons / Emojis** |
| Language  | **Python 3.10+** |

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/saasify.git
cd saasify
2️⃣ Create Virtual Environment
bash
Copy code
python -m venv venv
venv\Scripts\activate   # On Windows
# or
source venv/bin/activate  # On Mac/Linux
3️⃣ Install Dependencies
bash
Copy code
pip install -r requirements.txt
4️⃣ Apply Migrations
bash
Copy code
python manage.py makemigrations
python manage.py migrate
5️⃣ Create Superuser
bash
Copy code
python manage.py createsuperuser
6️⃣ Run Server
bash
Copy code
python manage.py runserver
➡️ Visit: http://127.0.0.1:8000/

## Dockerize The Application
## Just pull the Image from dockerhub and run command

-- Created Dockerfile
-- Created docker-compose file
   ## Run cmd-
      --docker-compose build --no-cache
      --docker-compose up
   

🔐 Authentication Flow
Default Route (/) → redirects to login page

Login Page → Enter credentials

Successful Login → Redirects to home

Incorrect Login → Displays “Invalid credentials” message

Signup Page → Registers new user

Logout → Redirects back to login with session cleared

👤 User Profile Management
Profile page includes:

Field	Description
Full Name	Editable
Email	Editable
Username	Read-only
Account Created	Auto

✅ Inline Edit Form to update Full Name and Email.
✅ Success message shown after update.
✅ Secured with @login_required.

💬 Contact Form
Accessible via /contact

Uses ContactForm and ContactMessage model

Saves data to DB

Displays success message on submission

📂 Static Files
Run this command to collect static files before deployment:

bash
Copy code
python manage.py collectstatic
Structure:

cpp
Copy code
static/
├── css/
│   └── login.css
└── images/
    └── avatar.png
🚀 Deployment Ready
🟢 Configured for production readiness
🟢 Uses Django Messages for user feedback
🟢 Easy to deploy on:

Render

Railway

Vercel (via Django adapter)

AWS / Azure / DigitalOcean

🤝 Contributing
We welcome contributions!
Follow these steps:


Copy code
# 1. Fork the repo
# 2. Create a new branch
git checkout -b feature-name

# 3. Commit changes
git commit -m "Added new feature"

# 4. Push
git push origin feature-name

# 5. Open a Pull Request 🚀
📄 License
This project is licensed under the MIT License.

👨‍💻 Author
Jahed Inamdar
Software Engineer 
🚀 Building SaaSify with Django, React, and Cloud

🌐 Connect: LinkedIn • GitHub
