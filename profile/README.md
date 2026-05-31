# Neo-Banker / 灵犀·Résonance Studio

> **For humans**: scroll to [What we build](#what-we-build).
> **For AI agents** (Claude Code / Cursor / Copilot CLI / etc.): see [AI agent quick-start](#ai-agent-quick-start) — every product repo has an `AGENT_HANDOFF.md` at root.

---

## What we build

Neobanker is a Hong Kong virtual-bank intelligence platform.

| Platform | Tagline |
|---|---|
| **灵犀 · Résonance Studio** | AI-based agent operating system — banking intelligence chatbot + dynamic dashboard |
| **璞炼 · Creuset Studio** | Data fusion platform (manual → copilot → autonomous) for ingesting + verifying + publishing banking knowledge |

---

## Repo map

| Repo | Purpose | Default branch | AI handoff |
|---|---|---|---|
| [**neobanker-dev-env**](https://github.com/neo-banker/neobanker-dev-env) | One-click cross-platform local dev env | `main` | [AGENT_HANDOFF.en.md](https://github.com/neo-banker/neobanker-dev-env/blob/main/AGENT_HANDOFF.en.md) |
| [**neobanker-agent**](https://github.com/neo-banker/neobanker-agent) | FastAPI conversational agent (multi-LLM, MCP server, region-aware) | `chatbot` | [AGENT_HANDOFF.en.md](https://github.com/neo-banker/neobanker-agent/blob/chatbot/AGENT_HANDOFF.en.md) |
| [**neobanker-frontend-MVP-V3**](https://github.com/neo-banker/neobanker-frontend-MVP-V3) | Next.js 14 frontend (Studio canvas + chatbot embed) | `chatbot` | [AGENT_HANDOFF.en.md](https://github.com/neo-banker/neobanker-frontend-MVP-V3/blob/chatbot/AGENT_HANDOFF.en.md) |
| [**neobanker-backend-MVP-V2**](https://github.com/neo-banker/neobanker-backend-MVP-V2) | Spring Boot 3.1 backend (MySQL + ES + Redis) | `main` | [AGENT_HANDOFF.en.md](https://github.com/neo-banker/neobanker-backend-MVP-V2/blob/main/AGENT_HANDOFF.en.md) |
| [neobanker-crawler](https://github.com/jajupmochi/neobanker-crawler) | Crawler agent (own org pending migration) | `main` | TBD |
| [creuset-studio](https://github.com/neo-banker/creuset-studio) | Data platform UI concept (brainstorm) | `main` | [AGENT_HANDOFF.en.md](https://github.com/neo-banker/creuset-studio/blob/main/AGENT_HANDOFF.en.md) |

---

## AI agent quick-start

> Drop any of these URLs in your AI agent of choice (Claude Code, Cursor, Copilot CLI, Aider, Cline, etc.):

**To bootstrap full-stack local dev environment:**
```
Read https://github.com/neo-banker/neobanker-dev-env/blob/main/docs/ai-agent-prompt.md and execute the bootstrap procedure.
```

**To continue work on a specific repo:**
```
Read https://github.com/neo-banker/<repo>/blob/<branch>/AGENT_HANDOFF.en.md and continue from NEXT ACTIONS.
```

Each `AGENT_HANDOFF.{md,en.md}` (CN + EN) contains:
- One-line state
- Read order (which docs to load first)
- Current branch + sync status
- NEXT ACTIONS (priority-ordered)
- Recently shipped (don't redo)
- Hard constraints (don't break)
- Cross-machine sync hints

---

## License

Internal — see each repo for specifics.

## Contact

- Engineering: see [neobanker-agent](https://github.com/neo-banker/neobanker-agent) Issues
- Compliance: see [neobanker-agent/docs/audiences/compliance/](https://github.com/neo-banker/neobanker-agent/tree/chatbot/docs/audiences/compliance)
