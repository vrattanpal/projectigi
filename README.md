# S.A.I. v2 — Super Artificial Intelligence Agent

S.A.I. v2 is a modular AI agent platform starter with:
- model-provider abstraction
- multi-step planning loop
- persistent memory
- tool registry
- web research tool
- safe local code execution
- workspace file tools
- GitHub integration interface
- modern Next.js UI

## Safety
Tool execution is explicit and sandbox-oriented. Do not expose arbitrary shell execution to an internet-facing deployment without authentication, isolation, resource limits, and approval controls.

## Run
Backend:
```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
uvicorn app.main:app --reload --port 8000
```

Frontend:
```bash
cd frontend
npm install
copy .env.local.example .env.local
npm run dev
```
