---
name: claude-ecosystem-scan
description: Vollständiger Claude Ökosystem Scanner — auf Nutzer-Query hin scannen GitHub+Marketplace, filtern nach Relevanz, zur Prüfung präsentieren, bei Approval installieren.
category: skill-development
version: 1.0.0
status: active
swarmId: swarm-1776493226884-s1ndhv
workflowId: workflow-1776493261570-3bm56r
templateId: template-1776493264636-nctzrg
---

# claude-ecosystem-scan

Ruflo Swarm mit 4 Agents. Vollständig orchestriert. RIFTERBOT isoliert.

## Agents

| Agent | Modell | Rolle |
|-------|--------|-------|
| `orchestrator` | Sonnet | Koordiniert, präsentiert, installiert |
| `github-scanner` | Haiku | Scannt GitHub Topics + Repos + Releases |
| `marketplace-scanner` | Haiku | Scannt claudemarketplaces.com + official plugins |
| `filter-agent` | Haiku | Filtert + bewertet nach Relevanz 0-10 |

## Workflow (6 Schritte)

```
1. query-intake       → Orchestrator empfängt deine Suchanfrage
2. parallel-scan      → GitHub + Marketplace gleichzeitig
3. filter-and-rank    → Filter-Agent bewertet nach deinen Kategorien
4. present-to-user    → Tabelle: Name | Kategorie | Score | Link skill.md
5. user-review        → Du liest, entscheidest
6. install-or-expand  → claude plugin install / MCP erweitern / Ruflo Connector
```

## Nutzung

Einfach schreiben:

```
"such mir Skills für Autonomie und TikTok Content Produktion"
"neue MCP Server für Finance und Data Science"
"was gibt es neues im Claude Ökosystem diese Woche"
```

## Scan-Quellen

- GitHub Topics: `claude-code-skill`, `mcp-server`, `claude-plugin`
- `wondelai/skills` — Releases + neue Commits
- `claudemarketplaces.com`
- `anthropics/claude-plugins-official`
- `anthropics/claude-code` — Releases + Changelog
- `modelcontextprotocol/servers` — neue MCP Server

## Kategorien (Peters Prioritäten)

1. Automation
2. Finance / Trading
3. Data Science
4. TikTok / Content Produktion
5. Skill Development

## Isolation

`rifterbot_isolation: true` — der Bot wird in keinem Schritt berührt.
