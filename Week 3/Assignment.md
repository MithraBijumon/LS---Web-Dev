# 🎬 Week 3 Assignment – Django Backend for YouTube Clone

Welcome to the backend era! This week, we're bringing your Week 2 YouTube Clone UI to life using Django.

---

## 🚀 Objective

Build a **functional Django backend** that enables:

- User registration and login
- Simulated email verification
- Protected user dashboard
- Clean Django admin panel
- Styled HTML forms using Bootstrap or custom CSS

> You'll plug this into your frontend in Week 4. For now, test via Django templates or DRF.

---

## 📦 Features Implemented

### 📝 1. User Registration
- Fields: `username`, `email`, `password`, `confirm password`
- Validations:
  - Email must be unique
  - Passwords must match
- Used `UserCreationForm` / custom `ModelForm`

---

### ✅ 2. Simulated Email Verification
- After registration, user redirected to a verification route:
```
/verify/<token>
```
- No actual email sent — simulated with console backend or dummy view
- Success message displayed: _“Account Verified Successfully”_

---

### 🔐 3. Login + Logout
- Used Django’s `authenticate()` and `login()`
- Handled wrong credentials with clear error messages
- Implemented logout functionality

---

### 🔒 4. Protected Dashboard
- Created a `/dashboard` view
- Used `@login_required` decorator
- Redirects unauthenticated users to login page

---

### ⚙️ 5. Django Admin Setup (✅ Mandatory)
- Registered all relevant models in `admin.py`
- Added:
- `list_display`
- `search_fields`
- `ordering`
- Organized fieldsets properly
- Optional: Customized admin CSS/colors for cleaner look

---

### 🖼️ 6. Styled HTML Pages
- Used Bootstrap for clean forms & UI
- Styled pages:
- `register.html`
- `login.html`
- `dashboard.html`
- `verify.html`
- Navbar added with login/logout buttons & login status

---

## 🗂 Folder Structure

```
youtube_auth/
├── manage.py
├── youtube_auth/
│ ├── settings.py
│ ├── urls.py
├── accounts/
│ ├── views.py
│ ├── urls.py
│ ├── forms.py
│ ├── models.py
│ ├── admin.py
│ └── templates/
│ ├── register.html
│ ├── login.html
│ ├── dashboard.html
│ └── verify.html
```
---

## 💎 Bonus Features (Optional)
- ✅ Django Messages: _“User created successfully ✅”_
- 🖼️ Profile image field (`ImageField` saved to `media/`)
- 🎬 Watch Later simulation using Django sessions
- ⏳ Loading animation for login/register pages

---

## 📤 Submission

- ✅ GitHub Repo: [your-repo-link]
- ✅ Short Video Walkthrough:
  - Registration + Verification flow
  - Login + Protected Dashboard
  - Django Admin showcase
  - Bonus features (if any)

---

## ✅ Requirements

- No code errors ❌
- Clean, styled templates 🌟
- Admin panel production-ready 🛠️

---

Let’s bring logic to life. Backend is here. 🔥
