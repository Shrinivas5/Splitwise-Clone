# Splitwise Clone

A full-stack expense-sharing application inspired by Splitwise. Create groups, record shared expenses, split costs, and track balances to understand who owes whom.

## ✨ Features

- Create and manage groups
- Add and manage expenses
- Equal and percentage-based expense splitting
- Automatic balance tracking
- REST API with FastAPI
- Responsive React UI with Tailwind CSS
- PostgreSQL with Docker Compose
- SQLite support for local development

## 🛠️ Tech Stack

**Backend:** Python, FastAPI, SQLAlchemy, Pydantic

**Frontend:** React, Tailwind CSS, Axios

**Database:** PostgreSQL / SQLite

**DevOps:** Docker, Docker Compose

## 🚀 Getting Started

### Option 1 — Docker Compose

```bash
git clone https://github.com/Shrinivas5/Splitwise-Clone.git
cd Splitwise-Clone
docker-compose up --build
```

The application will be available at:

- Frontend: http://localhost:3000
- Backend API: http://localhost:8000
- Swagger API Docs: http://localhost:8000/docs

### Option 2 — Local Development

#### Backend

```bash
cd backend
python -m venv venv
```

Windows:

```bash
.\venv\Scripts\activate
```

macOS/Linux:

```bash
source venv/bin/activate
```

Install dependencies and start the API:

```bash
pip install -r requirements.txt
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

#### Frontend

In a new terminal:

```bash
cd frontend
npm install
npm start
```

## 📁 Project Structure

```text
.
├── backend/
│   ├── app/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── routes/
│   │   └── main.py
│   ├── requirements.txt
│   └── Dockerfile
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.tsx
│   ├── package.json
│   └── Dockerfile
└── docker-compose.yml
```

## 🔌 API Documentation

FastAPI automatically provides interactive API documentation at:

http://localhost:8000/docs

## 📌 Notes

- Authentication and authorization are not included.
- Payment settlement is outside the scope of this project.
- SQLite is used for local development; Docker Compose uses PostgreSQL.
- Percentage-based splits must total 100%.

## 👨‍💻 Author

**Shrinivas D**  
GitHub: https://github.com/Shrinivas5
