# Favour Akintoye — The Compendium

A deliberately lean FastAPI application serving the existing Compendium frontend from one origin. There is no database, user account system, contact-message storage, or contact form in this version.

The contact compass already contains the public destinations (email, Substack, GitHub and Payla) in `static/app.js`. Those links work directly in the browser and do not need a backend database or configuration endpoint.

## Project structure

```text
.
├── backend/app/main.py   # FastAPI routes and static frontend hosting
├── static/               # HTML, CSS and JavaScript frontend
├── Dockerfile
├── railway.toml
├── render.yaml
└── requirements.txt
```

## Run locally

Python 3.11 or newer is recommended.

```bash
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
uvicorn backend.app.main:app --reload --host 127.0.0.1 --port 8000
```

Open `http://127.0.0.1:8000`. Health check: `http://127.0.0.1:8000/api/health`.

## API

| Method | Endpoint | Purpose |
|---|---|---|
| `GET` | `/api/health` | Confirms that the FastAPI application is running |

The API intentionally has no contact submission endpoint. The existing contact options are external destinations, not messages collected by this website.

## Deployment

The Dockerfile listens on the platform-provided `PORT`. Render and Railway configuration files include the health-check path. Connect the custom domain to the selected host and enable HTTPS. The frontend and API share the same origin, so CORS configuration is unnecessary.

No database service, database URL, SMTP credentials, or application secrets are required.

## Current boundaries

- All instruments, calculations, navigation and portfolio content remain client-side.
- FastAPI serves the static frontend and provides a health endpoint.
- Email opens the visitor's mail application using `mailto:`.
- Substack, GitHub and Payla open their respective external destinations.
- There is no admin panel or content-management API.
