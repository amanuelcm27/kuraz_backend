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
2. git clone 
3. pip install -r requirements.txt
4. python manage.py migrate
5. python manage.py runserver
# Example POST Request
POST /api/tasks
Content-Type: application/json

{
  "title": "Write documentation"
}
