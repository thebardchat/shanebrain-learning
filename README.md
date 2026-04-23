# ShaneBrain Learning

> Auto-learning inbox pipeline: drop a file in, it gets ingested to Weaviate on cron. Zero-friction knowledge capture for the ShaneBrain brain.

**Built by:** Shane Brazelton + Claude Anthropic (ShaneBrain ecosystem, Hazel Green AL)

Ingestion pipeline for ShaneBrain learning data.
Folders: inbox/ (new data), processed/ (ingested), logs/ (run logs).
Part of the ShaneBrain Core ecosystem.

## How It Works

1. Drop any document into `inbox/`
2. Cron picks it up automatically
3. Embeds with Ollama (nomic-embed-text, 768-dim)
4. Stores in Weaviate LegacyKnowledge collection
5. Moves to `processed/` — audit trail in `logs/`

## Tech Stack

- Python 3
- Weaviate (Docker, port 8080)
- Ollama (nomic-embed-text)
- Cron scheduling

## Constitution

This project operates under the [ShaneBrain Constitution](https://github.com/thebardchat/constitution/blob/main/CONSTITUTION.md). See [CONSTITUTION.md](./CONSTITUTION.md).

**GitHub Pages:** [thebardchat.github.io/shanebrain-learning](https://thebardchat.github.io/shanebrain-learning/)

---

Built with [Claude + ShaneBrain](https://claude.ai/referral/4fAMYN9Ing) — AI tools for humans who build.
