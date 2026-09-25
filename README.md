# Django ToDo App

A small task manager built with Django. Create tasks, edit them, mark them complete or incomplete, and remove tasks you no longer need.

## Features

- Add new tasks
- Edit an existing task
- Mark tasks as complete or incomplete
- Delete tasks
- Separate active and completed task lists
- SQLite database for local development

## Tech Stack

- Python
- Django 6.1
- SQLite
- Bootstrap 5

## Getting Started

### Prerequisites

- Python 3.10 or newer
- pip

### Installation

1. Clone the repository and enter the project directory.

   ```bash
   git clone https://github.com/hasansaylawala529-bit/TODO-Django.git
   cd TODO-Django
   ```

2. Create and activate a virtual environment.

   ```bash
   python -m venv env
   ```

   Windows PowerShell:

   ```powershell
   .\env\Scripts\Activate.ps1
   ```

   macOS/Linux:

   ```bash
   source env/bin/activate
   ```

3. Install Django.

   ```bash
   pip install "Django==6.1.1"
   ```

4. Apply database migrations.

   ```bash
   python manage.py migrate
   ```

5. Start the development server.

   ```bash
   python manage.py runserver
   ```

6. Open <http://127.0.0.1:8000/> in your browser.

## Project Structure

```text
todo/                 Task model, views, URLs, and migrations
todo_main/            Django project configuration
templates/            HTML templates
manage.py             Django management entry point
```

## Database

`db.sqlite3` is intentionally ignored by Git. Each developer creates a local database by running migrations, which keeps machine-specific task data out of the repository.

## Development Notes

This project uses Django's development settings. Before deploying, set `DEBUG = False`, provide a secure secret key through an environment variable, configure `ALLOWED_HOSTS`, and use a production-ready database and web server.

## License

This project is available for learning and personal use.
