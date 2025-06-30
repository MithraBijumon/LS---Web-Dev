# YouTube Clone (React + Django)

## 📌 Objective

Build a simple YouTube-like application with the ability to:

- ✅ Register, Login, Logout  
- ✅ Upload videos with title and description  
- ✅ View a list of uploaded videos  
- ✅ Watch videos on a dedicated video player page  
- ✅ Basic Navbar and Sidebar for navigation

---

## 🧩 Project Structure

ytclone/
│
├── backend/ # Django Backend
│ ├── backend/ # Django project directory
│ │ ├── init.py
│ │ ├── settings.py # Project settings
│ │ ├── urls.py # Main URL routing
│ │ ├── wsgi.py
│ │ └── asgi.py
│ │
│ ├── api/ # Django app for APIs
│ │ ├── migrations/ # DB migrations
│ │ ├── init.py
│ │ ├── admin.py # Admin site configs
│ │ ├── apps.py
│ │ ├── models.py # Models (User, Video)
│ │ ├── serializers.py # DRF Serializers
│ │ ├── views.py # API Views
│ │ ├── urls.py # API URL routing
│ │ └── tests.py # Tests (Optional)
│ │
│ ├── media/ # Uploaded media (videos, thumbnails)
│ ├── db.sqlite3 # Database (SQLite by default)
│ ├── manage.py # Django project manager
│
├── frontend/ # React Frontend
│ ├── public/ # Public files (index.html)
│ │ └── index.html
│ │
│ ├── src/ # React source code
│ │ ├── components/ # All React components
│ │ │ ├── Navbar.js # Navigation bar
│ │ │ ├── Sidebar.js # Sidebar menu
│ │ │ ├── Home.js # Display list of videos
│ │ │ ├── Upload.js # Upload video page
│ │ │ ├── Login.js # Login form
│ │ │ ├── Register.js # Register form
│ │ │ ├── VideoPlayer.js # Video watching page
│ │ │ └── Dashboard.js # User's uploaded videos
│ │ │
│ │ ├── App.js # Main app component with routing
│ │ ├── App.css # Global styles
│ │ ├── index.js # Entry point for React
│ │ └── axiosConfig.js # Axios instance setup (optional)
│ │
│ ├── package.json # Node dependencies for React
│ └── README.md # Frontend documentation (optional)
│
├── README.md # Main project documentation

yaml
Copy
Edit

---

## ⚙️ Project Breakdown

### 🔧 Backend (Django + DRF)

#### ✅ Setup

- Create Django project and an app (`api`)
- Install required libraries: Django Rest Framework, CORS

#### 🧱 Models

- **User** (default Django user)
- **Video**: user, title, description, video file, uploaded_at

#### 🧪 Serializers

- `UserSerializer`
- `VideoSerializer`

#### 🔍 Views

APIs to:

- Register user  
- Login user  
- Upload video  
- List videos  
- Fetch single video  

#### 🔗 URLs

- Connect APIs via router and `urls.py`

#### 🔄 CORS & Media

- Enable CORS for frontend  
- Configure media file handling for video uploads  

---

### 🖥️ Frontend (React)

#### ✅ Setup

- Create React app  
- Install Axios, React Router, Bootstrap (or simple CSS)

#### 📄 Pages/Components

- **Navbar**  
- **Sidebar**  
- **Home**: list all videos  
- **Upload**: form to upload video  
- **Login**: user login  
- **Register**: user signup  
- **VideoPlayer**: watch selected video  
- **Dashboard**: user's uploaded videos

#### 🛣️ Routing

- Setup routing with React Router for the above pages

#### 🔌 API Integration

- Use Axios to connect to Django backend APIs

#### 🎨 Basic Styling

- Keep minimal styling with Bootstrap or CSS  
- Optional: Add your own creativity for UI improvements

---

## 🔑 Key Functionalities to Implement

- User Authentication (Register/Login/Logout)  
- Video Upload with title and description  
- Display all videos on the home page  
- Play video on click (Video Player)  
- Dashboard to show user’s uploaded videos  
- Navbar + Sidebar for navigation  
- **Optional:** Watch Later functionality  

---

## 📚 YT Clone Resources

- [YouTube Tutorial Playlist](https://www.youtube.com/playlist?list=PLgWjD_CBfh0Daeqt-Q5ogwc9FPAsqH5sx)

---

> You can deploy this project — it is totally optional.
