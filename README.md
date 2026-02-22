# 🚀 Uniflow - Unified Tender Proposal Platform

A hackathon MVP for iteratively drafting tender proposals with a conversational interface.

## Quick Start

### Backend (Python/FastAPI)

```bash
cd backend
uv run uvicorn main:app --reload
```

Backend runs at: http://localhost:8000

### Frontend (React/Vite)

```bash
cd frontend
bun dev
```

Frontend runs at: http://localhost:5173

## Demo Credentials

- **Email:** demo@uniflow.com
- **Password:** demo123

## Features

- ✅ JWT-based authentication
- ✅ Create and manage proposals
- ✅ Iterative drafting with chat input
- ✅ Live Markdown preview
- ✅ Submit finalized proposals
- ✅ **Google Search grounding** - AI can search the web for real-time information
- ✅ File attachments (PDF, DOCX, Excel, Images)
- ✅ Team management and collaboration

> 📖 **New!** Check out [GOOGLE_SEARCH.md](./GOOGLE_SEARCH.md) for details on using Google Search in your proposals.


## Project Structure

```
uniflow/
├── backend/           # Python/FastAPI backend
│   └── main.py        # All API endpoints
├── frontend/          # React/Vite frontend
│   └── src/
│       ├── api/       # API client
│       ├── auth/      # Auth components
│       └── proposals/ # Proposal workspace
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/auth/login` | Login with email/password |
| GET | `/proposals` | List all proposals |
| POST | `/proposals` | Create new proposal |
| GET | `/proposals/{id}` | Get proposal by ID |
| POST | `/proposals/{id}/iterate` | Iterate on proposal |
| POST | `/proposals/{id}/submit` | Submit final proposal |
