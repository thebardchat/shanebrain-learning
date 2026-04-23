# Proto-Mega-Crew — The Original Multi-Agent Coordinator

**Historical Artifact — Do Not Delete**

This folder contains the original multi-agent coordinator that predates the current MEGA crew architecture.

## What It Is

`team_assemble.py` was the first multi-agent orchestration system built in the ShaneBrain ecosystem. Written in **December 2025**, it ran on Shane's laptop while he dispatched trucks for SRM Concrete out of Hazel Green, Alabama.

## Architecture

Uses the Anthropic API with specialist agent roles:
- **architect** — system design decisions
- **auth_specialist** — authentication and access control
- **api_developer** — endpoint construction
- **frontend_developer** — UI logic
- **database_engineer** — data modeling

`project_scan.py` — companion scanner that read the codebase and fed context to the agents.
`team_progress.json` — live state file tracking what each agent had completed.

## Legacy

This coordinator evolved directly into the current MEGA crew:
- Discord bot (`discord-bot/`)
- Arcade bot (`arcade-bot/`)
- Social bot (`social-bot/`)
- Buddy Claude (port 8008)

The specialist role pattern is still visible in how the MEGA crew divides responsibilities. This is where that pattern was born.

## Files

| File | Description |
|------|-------------|
| `team_assemble.py` | Original multi-agent orchestrator (Anthropic API) |
| `project_scan.py` | Codebase context scanner for agents |
| `team_progress.json` | Agent progress state snapshot |

---

Built by Shane Brazelton + Claude Anthropic | ShaneBrain Ecosystem, Hazel Green AL
