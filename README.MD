# 📝 Task Manager REST API

A simple backend-only Task Manager built with Django and Django REST Framework.

## 📌 Features

- Create, read, update (mark complete), and delete tasks
- Filter tasks by completion status (`completed=true/false`)
- Validation to ensure task titles are not empty

## 📂 Endpoints

| Method | Endpoint            | Description                    |
|--------|---------------------|--------------------------------|
| GET    | `/api/tasks`        | List all tasks                 |
| GET    | `/api/tasks?completed=true` | Filter completed tasks    |
| GET    | `/api/tasks?completed=false` | Filter pending tasks     |
| POST   | `/api/tasks`        | Add a new task                 |
| PUT    | `/api/tasks/<id>`   | Mark task as completed         |
| DELETE | `/api/tasks/<id>`   | Delete a task                  |

## 🧰 Setup Instructions

1. **Clone the project**
    git clone 
    pip install -r requirements.txt
    python manage.py migrate
    python manage.py runserver
# Example POST Request
POST /api/tasks
Content-Type: application/json

{
  "title": "Write documentation"
}
