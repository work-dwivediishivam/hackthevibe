# 🚀 Uniflow - Unified Tender Proposal Platform

A hackathon MVP for iteratively drafting tender proposals with a conversational interface.

## Quick Start for HackTheVibe Judges

Refer to the demo for application insights.

Go to the following link :-
```bash
https://uniflow-pqmm.vercel.app
```

Here are access logins to 2 users with different permission, refer to the demo video to test it out.
User 1 ->
```bash
User - tushar21211@iiitd.ac.in
Password - asdf1234
)```
User 2 ->
```bash
User - varsha21499@iiitd.ac.in
Password - asdf1234
```


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
