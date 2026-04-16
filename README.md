# Stage 1 Personal API

This is a minimal personal API built with FastAPI and prepared for deployment behind Nginx on a VPS.

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --host 127.0.0.1 --port 8001
```

For Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --host 127.0.0.1 --port 8001
```

## Endpoints

### GET /

```json
{
  "message": "API is running"
}
```

### GET /health

```json
{
  "message": "healthy"
}
```

### GET /me

```json
{
  "name": "Oluwagbade Odimayo",
  "email": "o.odimayo@gbadedata.com",
  "github": "https://github.com/gbadedata"
}
```

## Live URL

http://13.43.217.25