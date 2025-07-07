# File Manager Main

## Project Overview
File Manager is a web application built with Django that allows users to sign up, log in, and create blog posts. Users can upload files (PDF or Excel) with their posts, and the application extracts the content from these files automatically. Posts can be marked as public or private. Public posts are visible to all users on the home page, while private posts are only visible to their authors.

## Important Files and Their Functionalities

- **manage.py**: Django's command-line utility for administrative tasks such as running the server, migrations, and more.
- **blog_app/settings.py**: Contains the project settings including database configuration, installed apps, middleware, and static files settings.
- **blog/urls.py**: Defines the URL routes and maps them to corresponding view functions.
- **blog/views.py**: Contains the main logic for handling user requests such as signup, login, logout, creating new posts, and displaying posts.
- **blog/models.py**: Defines the data models, including the `Post` model which represents blog posts with fields like title, content, file upload, author, and visibility.
- **blog/templates/blog/**: Contains HTML templates for rendering the web pages such as login, signup, home, new post, and user posts.
- **blog/static/**: Contains static assets like images used in the project.

## Requirements

To run this project, you need the following installed on your system:

- Python (version 3.8 or higher recommended)
- Django (version 4.2.3)
- PyPDF2 (for extracting text from PDF files)
- pandas (for extracting text from Excel files)

You can install the Python packages using pip:

```bash
pip install django==4.2.3 PyPDF2 pandas
```

## How to Run

1. Clone the repository or download the project files.
2. Navigate to the project directory in your terminal.
3. (Optional but recommended) Create and activate a virtual environment:

```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

4. Install the required packages:

```bash
pip install django==4.2.3 PyPDF2 pandas
```

5. Apply database migrations:

```bash
python manage.py migrate
```

6. Run the development server:

```bash
python manage.py runserver
```

7. Open your web browser and go to `http://***` to access the application.

---

This README provides a simple overview for non-developers to understand the project structure, important files, requirements, and how to get started.
