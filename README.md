# Secure Task Management Web Application (IKB21503)

A secure, scalable solution for managing Inventory in an organization.

---
### 1. Project Description

The Secure Task App is a Django-based web application developed for the course IKB21503 Secure Software Development at UniKL MIIT. This system is designed to allow users to manage personal tasks securely while enforcing proper security controls and Role-Based Access Control (RBAC) between normal users and administrators.

---
### 2. Team Members
   
1) HUWAINA YASMIN BINTI ANUAR ASFANDI (52215124317)

2) MUHAMMAD RUSMAN HILMI BIN MOHD RAIS (52215124426)

3) MUHAMAD AZIM SYAFAWI BIN ABDULLAH (52215124282)

4) MUHAMMAD SYAHMI BIN MOHD REZAL (52215124061)

---
### 3. Security Features Summary (OWASP Aligned)
In compliance with OWASP Top 10 and ASVS requirements, the following security features have been implemented:

1) Authentication: Secure login/logout using Django's built-in framework with Argon2 password hashing.

2) Access Control: Role-Based Access Control (RBAC) to restrict administrative functions (e.g., Audit Logs) to authorized users only.

3) Input Validation: Server-side validation using Django Forms to mitigate XSS and Injection attacks.

4) Database Security: Prevention of SQL Injection through the use of Django ORM for all database interactions.

5) Session Management: Protection against session hijacking via HttpOnly and Secure cookie flags.

6) CSRF Protection: Middleware and tokens enforced for all state-changing requests.

7) Error Handling: Custom 400, 403, 404, and 500 pages to prevent information leakage.

8) Secret Management: Sensitive configuration (e.g., SECRET_KEY) stored in environment variables (.env).

9) Audit Logging: Comprehensive logging of security-relevant events such as logins and task operations.

---
### 4. Installation Steps
  
#### 1.Clone the project:
```bash
git clone https://github.com/muhammadrusmanhilmi-boop/Cloud-Inventory-System.git
```
#### 2.Set up Virtual Environment
```bash 
python -m venv venv venv\Scripts\activate # For Windows
```
#### 3.Install Dependencies:
```bash 
pip install -r requirements.txt
```
#### 4.Environment Configuration:
```bash 
Create a .env file based on .env.example and set your SECRET_KEY and DEBUG=False
```
#### 5.Run Migrations
```bash 
python manage.py migrate
```
#### 6.Start Application 
```bash 
python manage.py runserver
```
