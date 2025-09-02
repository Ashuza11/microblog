# Microblog

A simple microblogging web application built with Flask.

## Features

- User registration and authentication
- Login/logout functionality
- User profile pages
- Posting messages (microblog posts)
- Secure password hashing
- Form validation
- Database migrations (with Alembic)
- Modern Flask best practices

## Tech Stack

- **Python 3**
- **Flask**
- **Flask-Login**
- **Flask-WTF**
- **SQLAlchemy**
- **Alembic** (for migrations)

## Getting Started

### Prerequisites

- Python 3.x
- pip

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/microblog.git
   cd microblog
   ```

2. Create a virtual environment and activate it:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set environment variables (optional, for development):

   ```bash
   export FLASK_APP=microblog.py
   export FLASK_ENV=development
   ```

5. Initialize the database:
   ```bash
   flask db upgrade
   ```

### Running the App

Start the development server:

```bash
flask run
```

Visit [http://localhost:5000](http://localhost:5000) in your browser.

## Project Structure

```
microblog/
│
├── app/
│   ├── __init__.py
│   ├── models.py
│   ├── forms.py
│   ├── routes.py
│   └── templates/
│       ├── base.html
│       ├── index.html
│       ├── login.html
│       └── register.html
├── migrations/
├── microblog.py
├── config.py
└── README.md
```

- `app/`: Contains the main application code, including models, forms, routes, and templates.
- `migrations/`: Stores database migration files managed by Alembic.
- `microblog.py`: The entry point for the Flask application.
- `config.py`: Configuration settings for the application.
- `README.md`: Documentation for the project.

## License

This project is licensed under the MIT License.

Feel free to customize this README with additional details or instructions as needed!
