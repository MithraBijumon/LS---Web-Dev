# 🐍 What is Django?

**Django** is a high-level Python web framework that promotes rapid development and clean, pragmatic design. Built by experienced developers, Django takes care of much of the hassle of web development, so you can focus on writing your app without reinventing the wheel.

It follows the **Model-View-Template (MVT)** architectural pattern and includes many built-in features such as authentication, admin interface, ORM, and more.

---

## ✅ Benefits of Django

| Feature             | Description                                                             |
|---------------------|-------------------------------------------------------------------------|
| 🔐 Secure            | Protects against threats like SQL injection, CSRF, XSS, etc.           |
| ✨ Rapid Development | Built-in admin, ORM, and other features reduce development time.       |
| 🚀 Scalable          | Used by large-scale companies such as Instagram and Pinterest.         |
| 🧰 Modular           | Follows a modular architecture and supports reusable components.       |
| 🛠️ Admin Interface   | Automatically generates admin dashboard from models.                   |
| 🔍 ORM               | Allows database interaction using Python code instead of SQL.          |

---

## 💡 Real-Life Examples Using Django

| Website              | Description                                          |
|----------------------|------------------------------------------------------|
| 🌐 Instagram          | Uses Django for backend services.                    |
| 📰 The Washington Post | Manages large volumes of editorial content.         |
| 💬 Disqus             | Built its entire comment platform using Django.     |

---

## 🚀 How to Set Up Django (Step-by-Step)

### 📌 Prerequisites
- Python 3.8+
- Basic knowledge of Python programming

### ⚙️ Step 1: Install Virtual Environment (Optional)
```bash
pip install virtualenv
virtualenv venv
```
Activate it:
```bash
# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate
```

### ⚙️ Step 2: Install Django
```bash
pip install django
django-admin --version
```

### ⚙️ Step 3: Create a Django Project
```bash
django-admin startproject mysite
cd mysite
python manage.py runserver
```
Open in browser: [http://127.0.0.1:8000](http://127.0.0.1:8000)

### ⚙️ Step 4: Create a Django App
```bash
python manage.py startapp blog
```
Add `'blog'` to `INSTALLED_APPS` in `mysite/settings.py`

### ⚙️ Step 5: Run Migrations
```bash
python manage.py migrate
```

### ⚙️ Step 6: Create Admin User (Optional)
```bash
python manage.py createsuperuser
```

---

## 🐍 Django Video Learning Resources

- 🔹 [Django One Shot in English](https://youtu.be/PtQiiknWUcI?si=7eenzVR29bCYD-0P)
Follow this timeline:
   | **Topic**                      | **Time Start**         |
|-------------------------------|------------------------|
| What is Django                | 5:27                   |
| Installation & Setup          | 15:59                  |
| Views & URLs                  | 31:28                  |
| Templates                     | 39:55                  |
| Admin Panel & Database        | 1:04:25                |
| CRUD Operations               | 1:39:00                |
| User Auth (Login, Logout)     | 2:22:27 → 2:39:03      |

- 🔹 [Basic Overview in English (after 22:00 min)](https://youtu.be/rHux0gMZ3Eg?si=0TB_P5_seRAXyGIC)
- 🔹 [Admin Panel](https://youtu.be/iLhcV7t3zug?si=nGbxyNHy25nV-kPh)
- 🔸 [Django Tutorial in Hindi](https://youtu.be/JxzZxdht-XY?si=i4PaPNe4kzVm2p29)

## Reading Resources

- 📖 [W3Schools Django](https://www.w3schools.com/django/)
- 📖 [GeeksforGeeks Django](https://www.geeksforgeeks.org/python/django-tutorial/)


- 🎓 [Guided Project (Optional)](https://youtu.be/Bu8_77S9w6g?si=2JkmBAfOZ3bWzmJr)

---

# ⚡️ Django REST API & JWT Authentication – Secure Your Backend Like a Pro

## 🔍 What is Django REST Framework (DRF)?

Django REST Framework is a toolkit that helps you build Web APIs using Django models and views. It allows your backend to communicate with the frontend (React here) or even external services by exposing JSON data over HTTP.

It works by converting your Django models into serializable data (like JSON), which can then be accessed and modified by API views and routes.

### 🔑 Key Components:
- **Serializers** – Convert Django models to/from JSON
- **API Views** – Endpoints that respond with data, not HTML
- **Routers** – Automatically generate URLs for views
- **Browsable Interface** – Lets you test APIs in your browser

Once you’ve defined your models and serializers, DRF allows you to perform CRUD operations — Create, Read, Update, and Delete — through standard HTTP methods (GET, POST, PUT, DELETE).

---

## 🔐 Authentication in Django REST Framework

### 🔍 How Does Authentication Work in APIs?
Authentication ensures that a user is who they claim to be. Django REST Framework provides multiple authentication mechanisms:

- **Session Authentication** – Uses Django’s default session and cookies
- **Basic Authentication** – Credentials passed with every request
- **Token Authentication** – Unique token passed in headers with requests

---

## 📘 Resources for Django REST API

- 📖 [DRF Authentication Guide](https://www.django-rest-framework.org/api-guide/authentication/)
- 📖 [Google Doc Guide](https://docs.google.com/document/d/1OmpeaJ5taUpJBPYLTr6krOwfuiGiyfkljJD3OjDbu9o/edit?usp=sharing)
- ▶️ [Video (Overview)](https://youtu.be/OTnuTerIUlo?si=LaEySnVLjiVPR3RX)
- ▶️ [Crash Course – English](https://youtu.be/NoLF7Dlu5mc?si=1qT6PcJGLSui5M0a)
- ▶️ [Full Tutorial – English](https://youtu.be/t-uAgI-AUxc?si=4tNm0zH8sn-pXbwe)
- ▶️ [Playlist – Hindi](https://youtu.be/DNFTUtZf1Zc?si=eYclIuA4hJ_mBJcC)

---

# 🔑 JWT Authentication – Stateless and Secure Login System

## 🔍 What is JWT and Why Use It?

JWT (JSON Web Token) is a modern, stateless, token-based authentication system. It’s especially useful when you're building APIs accessed by JavaScript apps, mobile apps, or other clients.

When a user logs in, the server returns:
- **Access Token** – Used for authenticating each request (short-lived)
- **Refresh Token** – Used to obtain a new access token when expired

---

## 📘 JWT Authentication Resources

- 📖 [DRF Auth Docs](https://www.django-rest-framework.org/api-guide/authentication/)
- ▶️ [JWT Auth – English](https://youtu.be/Xp0-Yy5ow5k?si=4_Qphsne0T2jhCn0)
- ▶️ [JWT Auth – Hindi](https://youtu.be/fXOKBbnMQow?si=iOHoNpMTULFgAAID)

---

🧡 *Created with ❤️ by WnCC*

**Stay consistent. Practice daily. Your backend journey has just begun.**

