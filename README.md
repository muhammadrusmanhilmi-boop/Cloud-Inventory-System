# Secure_Cloud_Inventory_System

A secure, scalable solution for managing Inventory in an organization.

---

## How to Run

### 1. Navigate to the project directory:
```bash
cd C:\Users\YourName\Path\To\secure-django-app
```

### 2. Run the application:
```Bash
venv\Scripts\activate
```

### 3. Run the server
```bash
python manage.py runserver
```

### 4. Access the application:
```bash
Open your browser and navigate to http://127.0.0.1:8000/home/.
```
---
Default Credentials

The application seeds a default Administrator account on startup:

Email: admin

Password: admin

---
Features

Role-Based Access Control (RBAC): Admin vs User Non-admin Roles.

Authorization Checks: Every endpoint verifies authorisation.

Audit Logs: Administrators are able to view activity and who attempted to log in.

Security: Secure login flow, Password, Session Management & CSRF Protection.
