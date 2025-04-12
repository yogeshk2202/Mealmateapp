![GitHub repo size](https://img.shields.io/github/repo-size/yogeshk2202/Mealmateapp)
![GitHub stars](https://img.shields.io/github/stars/yogeshk2202/Mealmateapp?style=social)
![GitHub forks](https://img.shields.io/github/forks/yogeshk2202/Mealmateapp?style=social)
![GitHub last commit](https://img.shields.io/github/last-commit/yogeshk2202/Mealmateapp)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

# 🍽️ Mealmate - Online Food Ordering System

**Mealmate** is a Django-based web application that enables users to register as **restaurant owners** or **customers**.  
- Restaurant owners can manage their restaurants and menus.  
- Customers can browse menus, add items to their cart, place orders, and pay using **Razorpay**.

---

## 🚀 Features

### 🔐 Authentication
- User registration & login (Restaurant Owner & Customer)
- Secure authentication using Django's built-in system

### 🏪 Restaurant Management
- Add, edit, and delete restaurants

### 📋 Menu & Orders
- Customers can browse menus
- Add items to cart and place orders

### 💳 Payment Integration
- Razorpay integration for secure online payments

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yogeshk2202/Mealmateapp.git
cd Mealmateapp

Set Up a Virtual Environment

python -m venv venv
venv\Scripts\activate          # For Windows
# OR
source venv/bin/activate       # For Mac/Linux

. Install Dependencies
pip install -r requirements.txt

Apply Migrations
python manage.py migrate

Create a Superuser
python manage.py createsuperuser

Run the Development Server
python manage.py runserver
Visit: http://127.0.0.1:8000/

📁 Directory Structure
mealmate/
│
├── delivery/
│   ├── migrations/
│   ├── static/delivery/css/style.css
│   ├── templates/delivery/
│   │   ├── add_res.html
│   │   ├── base.html
│   │   ├── checkout.html
│   │   ├── cusmenu.html
│   │   ├── customer_home.html
│   │   ├── display_res.html
│   │   ├── failed.html
│   │   ├── index.html
│   │   ├── menu.html
│   │   ├── orders.html
│   │   ├── show_cart.html
│   │   ├── sign_in.html
│   │   ├── sign_up.html
│   │   ├── success.html
│   │   └── userdata.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── manage.py
├── requirements.txt
└── mealmate/
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    └── wsgi.py


### 🔌 API Endpoints (If Using Django REST Framework)

| Method | Endpoint                      | Description                |
|--------|-------------------------------|----------------------------|
| GET    | `/restaurants/`               | List all restaurants       |
| POST   | `/restaurants/add/`           | Add a new restaurant       |
| PUT    | `/restaurants/update/<id>/`   | Update restaurant details  |
| DELETE | `/restaurants/delete/<id>/`   | Delete a restaurant        |
| GET    | `/menu/`                      | Get menu items             |
| POST   | `/order/`                     | Place an order             |

💰 Razorpay Payment Integration
1.Sign up at Razorpay

2.Get API keys from Razorpay Dashboard

3.Add the following to your settings.py:

RAZORPAY_KEY_ID = "your_key_id"
RAZORPAY_KEY_SECRET = "your_key_secret"

📫 Contact
Made with ❤️ by Yogesh K

