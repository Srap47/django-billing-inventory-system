# 💼 Billing & Inventory Management System (Django)

A **full-stack Django Billing & Inventory Management System** that automates essential business workflows — from billing and stock tracking to customer payments and analytics.  
Designed for small to medium enterprises (SMEs), this system helps manage sales operations with real-time insights and PDF invoice generation. :contentReference[oaicite:1]{index=1}

---

## 🚀 Key Features

- 🔐 **User Authentication** – Secure login for admin and staff  
- 👥 **Customer Management** – Maintain customer profiles and history  
- 📦 **Product & Inventory Control** – Track stock levels and auto-adjust on billing  
- 🧾 **Invoice & Billing** – Create, view, and generate PDF invoices  
- 💳 **Payment Tracking** – Record payments (cash, UPI, card, bank)  
- 📊 **Sales Analytics Dashboard** – Visualize revenue trends, top products, and stock movement  
- 🕓 **Timezone-aware Timestamps** – Consistent local time tracking  
- 🖥️ **Responsive UI** – Built with Bootstrap 5 for cross-device compatibility  
- 📁 **Modular Django Apps** – Clear separation of core modules for flexibility  



---

## 🧠 Tech Stack

| Layer         | Technology                  |
|---------------|-----------------------------|
| **Backend**   | Python, Django              |
| **Frontend**  | HTML5, CSS3, Bootstrap 5    |
| **Database**  | MySQL / Django ORM          |
| **PDF Invoicing** | WeasyPrint / xhtml2pdf |
| **Analytics** | Plotly Dash                 |
| **Development** | Git, GitHub, VS Code      |
| **Testing & Tools** | Postman                 |

---

## 📂 Project Structure

billing_system/
│
├── core/ # Main application modules
│ ├── models.py # Database models
│ ├── views.py # Views & business logic
│ ├── urls.py # App routes
│ ├── templates/ # HTML templates
│ └── static/ # CSS, JS, images
│
├── billing_system/ # Django project config
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
│
└── manage.py # Django CLI entrypoint

---

## ⚙️ Installation

### 1. Clone the Repo
```bash
cd Billing-software

2. Setup Virtual Environment

python3 -m venv venv
source venv/bin/activate     # Mac/Linux
venv\Scripts\activate        # Windows

3. Install Dependencies

pip install -r requirements.txt

4. Configure Database

Update settings.py with your MySQL credentials:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': '<your_db>',
        'USER': '<your_user>',
        'PASSWORD': '<your_password>',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}

Migrate models:

python manage.py makemigrations
python manage.py migrate

5. Create Admin User

python manage.py createsuperuser

6. Run the App

python manage.py runserver

Visit 👉 http://127.0.0.1:8000/
🧾 Invoice Logic Overview

    Invoice item quantity must not exceed available stock

    On billing, stock is automatically updated

    Deleting an invoice item restores stock

    PDF invoices can be exported or printed

(Expand based on specific logic implemented in your views and models)
📊 Analytics Dashboard

Visual insights include:

    Daily and category-wise sales trends

    Revenue and profit visualization

    Best-selling products

    Inventory movement charts

(Include sample dashboard screenshots here if available)
💡 Future Enhancements

You may consider adding:

    🛒 Role-based access control (Admin/Staff rights)

    📦 Supplier & Purchase management

    🔔 Low stock alerts

    🔄 REST API support (Django REST Framework)

    ☁️ Deployment via Docker / CI/CD

🤝 Contributing

Thanks for your interest! To contribute:

    ⭐ Star the repository

    🔱 Fork it

    ✨ Create a feature branch (git checkout -b feature/xyz)

    🛠️ Commit your changes

    🔃 Push to your branch

    📩 Open a pull request

👨‍💻 Author & Maintainers

## 👤 Author
**Sohom Banerjee**
- Git: https://github.com/Srap47
- Email: sohommister@gmail.com

Licensed under the MIT License — free to use and modify for personal or commercial projects.

⭐ If this project helped you, please give it a star!
