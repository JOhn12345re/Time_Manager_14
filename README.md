# Time Manager

Time tracking application split into a Django API and a React frontend.

## Project structure

- **Backend** — [`backend/`](./backend) — **Django 6.1** (Python)
- **Frontend** — [`frontend/`](./frontend) — **React 19** with **Vite 8**

## Backend (Django)

The virtual environment lives in `backend/venv`. Activate it **before** any Django or pip command:

```bash
cd backend
source venv/bin/activate
```

If the venv does not exist yet:

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
```

Install Python packages **inside the activated venv**:

```bash
pip install -r requirements.txt
```

Run the server (venv must be active):

```bash
python manage.py runserver
```

Deactivate the venv when you are done:

```bash
deactivate
```

## Frontend (React + Vite)

```bash
cd frontend
npm install
npm run dev
```

## Commit convention

Use one of these prefixes, followed by ` : ` and a short description of **what** changed:

| Prefix | When to use |
| --- | --- |
| `Init` | Project bootstrap, first setup of a tool or environment |
| `Feat` | New feature |
| `Fix` | Bug fix |
| `Doc` | Documentation only |
| `Refacto` | Code restructure with no behavior change |

Examples:

```
Init : install and configure django with venv
Feat : add clock-in endpoint
Fix : correct overtime calculation
Doc : update README setup steps
Refacto : extract time helpers from views
```
