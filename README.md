# LoanMe Backend API

A robust Django REST API powering a loan management system. This application provides endpoints for account management and loan processing.

## Features
- **User Authentication:** Secure access using JWT (JSON Web Tokens).
- **Loan Processing:** API endpoints to manage, apply, and track loans.
- **RESTful Architecture:** Built with Django REST Framework (DRF).
- **API Documentation:** Interactive Swagger documentation integrated via `drf-yasg`.
- **Production Ready:** Configured with Whitenoise and Gunicorn for easy deployment to Heroku or similar PaaS.

## Prerequisites
- Python 3.8+
- PostgreSQL or SQLite (local testing)

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/AbdlKabeer/loanme-backend.git
   cd loanme-backend
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Variables**
   Create a `.env` file in the root directory and add necessary variables such as `SECRET_KEY`, `DEBUG`, and `DATABASE_URL` (if using PostgreSQL).

5. **Run Migrations**
   ```bash
   python manage.py migrate
   ```

6. **Start the Development Server**
   ```bash
   python manage.py runserver
   ```
