# Online Shop

A Django-based e-commerce web application featuring user authentication, role-based access control, product management, and a shopping cart system with virtual currency support.

---

## Features
- **User Management** - registration, login, authentication and profile editing.
- **Role-based permissions** - Admins: Full system access | Employees: Product catalog management | Customers: Browse products, manage cart and purchase items using in-app currency
- **Products Management** - Product catalog management with role-based access, allowing admins and employees to create, update, and delete products, while all users can browse the catalog.
- **Shopping Cart & Purchases** - Shopping cart functionality enabling users to add and remove products, view total cost, and complete purchases using an virtual currency with balance validation.

---

## Tech Stack

- **Backend**: Django 5.x, Django ORM, PostgreSQL  
- **Frontend**: Django Templates, HTML, CSS, JavaScript  
- **Other Tools**: PyCharm, Git

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/PavelKalchishkov/Online-Shop.git
   cd Soft-Final-Project
   cd OnlineShopApp

2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   .venv/scripts/activate
   
3. Install dependencies:
   ```bash
   pip install -r requirements.txt

4. Set up PostgreSQL database in main folder(OnlineShopApp) settings.py:
DATABASES = {
    'default': {
        'ENGINE': '...',
        'NAME': '...',
        'USER': '...',
        'PASSWORD': '...',
        'HOST': '...',
        'PORT': '...'
    }
}

5. Apply migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate

6. Create a superuser (admin account):
   ```bash
   python manage.py createsuperuser

7. Run developement server:
   ```bash
   python manage.py runserver

8. Access the app at http://localhost:8000
