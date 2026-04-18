---
name: claude-ecosystem-scan
description: Vollständiger wöchentlicher Scan des Claude-Ökosystems — neue Skills, MCP-Server, Extensions, Tools und Anthropic-Updates die Claude besser machen. Kategorien: Automation, Finance, Data Science, Skill Development.
category: skill-development
version: 0.1.0
status: stub
---

# claude-ecosystem-scan

Wenn dieser Skill aufgerufen wird, scannt er folgende Quellen vollständig:

## Quellen

### Skills & Plugins
- `wondelai/skills` — neue Commits/Releases seit letztem Scan
- `anthropics/claude-plugins-official` — offizielle Plugin-Updates
- `claudemarketplaces.com` — neue Einträge
- GitHub Topic `claude-code-skill` — Community-Skills

### MCP Server (Model Context Protocol)
- `modelcontextprotocol/servers` — neue offizielle MCP-Server
- GitHub Topic `mcp-server` — neue Community-Server
- Kategorien prüfen: Browser, Database, Finance, Productivity, Dev Tools

### Anthropic Updates
- `anthropics/claude-code` Releases — neue Claude Code Features
- Anthropic Blog/Changelog — neue Modell-Features, API-Updates
- Claude Code Docs Changelog

### Community & Tools
- GitHub Topic `claude-code` — neue Repos mit hoher Aktivität
- Awesome-Claude Listen

## Filter-Kategorien (Peters Prioritäten)

1. **Automation** — Workflow-Automatisierung, Scheduling, Triggers
2. **Finance/Trading** — Market Data, Portfolio, Analytics
3. **Data Science** — Datenanalyse, Visualisierung, ML-Tools
4. **Skill Development** — Lerntools, Coaching, Produktivität

## Ausgabe-Format

```
CLAUDE ECOSYSTEM SCAN — [Datum]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

NEU SEIT LETZTEM SCAN:
Skills:    X neue
MCP:       X neue Server
Features:  X neue Claude Code Features

TOP PICKS für dich:
1. [Name] — [Kategorie] — [Warum relevant]
2. ...

BEREITS INSTALLIERT die updated wurden:
- ...
```

## Trigger

```
/claude-ecosystem-scan
```
