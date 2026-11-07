# JobPilot

A multi-agent job-hunt assistant. It collects job posts, scores them against a CV, drafts tailored applications, waits for human approval, then logs each application.

I'm building it to learn agentic AI engineering, one module at a time. See the [roadmap](docs/ROADMAP.md) and [progress](PROGRESS.md).

**Status:** Module 0 (setup). No agents yet.

## Run locally

You need Node 24+, pnpm 11 and Docker.

1. Create your env file:

   ```bash
   cp .env.example .env
   ```

2. In `.env`, replace each `change-me` with its own output from `openssl rand -hex 32`. Use the `JOBPILOT_DB_PASSWORD` value inside `DATABASE_URL` too.

3. Start the database and Langfuse:

   ```bash
   docker compose up -d
   ```

| Service | Address |
| --- | --- |
| JobPilot Postgres + pgvector | `localhost:5433` |
| Langfuse UI | http://localhost:3100 |

## Architecture, eval scores and cost numbers

Coming as the modules are finished.
