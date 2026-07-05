# Neo-Banker · Neobanker 信息平台 × Neo Horizon 梵净台 × Creuset 璞炼

> Hong Kong virtual-bank intelligence organisation. **Three platforms:**
> - 🏦 **Neobanker (信息平台)** — the root **information platform**: bank/fintech intelligence (data dashboard + REST APIs + data model).
> - 🌅 **Neo Horizon (梵净台)** — the **AI-assistant platform**. An **independent** platform, currently mounted under the information platform's `assistant` subdomain (may be split out later).
> - 🧪 **Creuset (璞炼)** — the **data-fusion platform**: ingest → verify → publish banking knowledge.
>
> **Newcomers / 新人** → start from the role-based entry: **[Neobanker docs · role nav](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/audiences/README.md)** · for Creuset see **[creuset-docs](https://github.com/neo-banker/creuset-docs)**.
> **AI agents** (Claude Code / Cursor / Copilot …) → see [AI agent quick-start](#ai-agent-quick-start); every product repo has an `AGENT_HANDOFF.md` at its root.

## Dev · test · deploy flow

`feature → PR → develop → (staging auto-deploy + auto-seed) → PR → main → prod`. **`main` and `develop` are PR-only** (enforced by a pre-push hook). See [branch-workflow](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/standards/branch-workflow.md) + [native-staging](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/standards/native-staging.md).

## Repositories

### 🏦 Neobanker + 🌅 Neo Horizon
| Repo | Purpose | Stack |
|---|---|---|
| [**neobanker-docs**](https://github.com/neo-banker/neobanker-docs) | Central docs hub + role-based entry | Markdown |
| [**neobanker-frontend-MVP-V3**](https://github.com/neo-banker/neobanker-frontend-MVP-V3) | Next.js dashboard + Neo Horizon AI Studio canvas | Next.js / React / TS / Tailwind / Clerk |
| [**neobanker-backend-MVP-V2**](https://github.com/neo-banker/neobanker-backend-MVP-V2) | Spring Boot REST + data model | Spring Boot 3.1 / Java 17 / MySQL |
| [**neobanker-agent**](https://github.com/neo-banker/neobanker-agent) | FastAPI AI agent (Neo Horizon assistant) | FastAPI / Python 3.12 / uv |
| [**neobanker-crawler**](https://github.com/neo-banker/neobanker-crawler) | FastAPI ingestion control-plane | FastAPI / Python 3.12 |
| [**neobanker-dev-env**](https://github.com/neo-banker/neobanker-dev-env) | One-click local docker stack + CICD templates + staging scripts | Shell / docker compose |
| [**neobanker-data**](https://github.com/neo-banker/neobanker-data) | Dataset SSOT + data docs + scratch | CSV / SQL / docs |

### 🧪 Creuset
| Repo | Purpose |
|---|---|
| [**creuset-docs**](https://github.com/neo-banker/creuset-docs) | Creuset central docs hub |
| creuset-{frontend,backend,agent,crawler,dev-env} | Data-platform services (mirror the Neobanker structure) |

> **Pinned** (org homepage): neobanker-docs · neobanker-frontend-MVP-V3 · neobanker-backend-MVP-V2 · neobanker-agent · neobanker-dev-env (adjust in org settings).

## AI agent quick-start

> Drop a URL into your AI agent of choice:

**Bootstrap the full local dev environment:**
```
Read https://github.com/neo-banker/neobanker-dev-env/blob/main/docs/ai-agent-prompt.md and execute the bootstrap procedure.
```
**Continue work in a specific repo:**
```
Read https://github.com/neo-banker/<repo>/blob/<branch>/AGENT_HANDOFF.en.md and continue from NEXT ACTIONS.
```
Each `AGENT_HANDOFF.{md,en.md}` (中文 + English) holds: one-line state · read order · current branch · NEXT ACTIONS · shipped (don't redo) · hard constraints.

<details>
<summary><b>中文版（点开）</b></summary>

香港虚拟银行情报组织，旗下**三个平台**：

- 🏦 **信息平台 Neobanker** —— 根/主平台（银行/金融情报：数据看板 + REST API + 数据模型）。
- 🌅 **梵净台 Neo Horizon** —— **AI assistant 平台**。**独立平台**，当前挂在信息平台的 `assistant` 子域下（未来可能拆出）。
- 🧪 **璞炼 Creuset** —— **数据融合平台**（抓取 → 校验 → 发布）。

**新人**：先按角色进入 —— [Neobanker 角色导航](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/audiences/README.md)；Creuset 见 [creuset-docs](https://github.com/neo-banker/creuset-docs)。

**开发/测试/部署流程**：`feature → PR → develop →（staging 自动部署 + 自动播种）→ PR → main → 生产`。**main/develop 只能走 PR**（pre-push 钩子强制）。见 [分支流程](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/standards/branch-workflow.md) 与 [原生 staging](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/standards/native-staging.md)。

仓库地图见上方英文表；置顶建议：docs 枢纽 + 前端 + 后端 + agent + dev-env。

</details>

## License · Contact
Internal project — see each repo. Engineering → the relevant repo's Issues; Compliance → [neobanker-docs compliance](https://github.com/neo-banker/neobanker-docs/blob/main/docs/platform/audiences/compliance/compliance-brief.md).
