---
name: claude-skill-audit
description: Zeigt vollstaendig was aktuell installiert ist (Skills, MCP, Plugins) und vergleicht mit dem Oekosystem. Luecken, veraltete Versionen, Upgrade-Empfehlungen.
category: skill-development
version: 0.1.0
status: stub
---

# claude-skill-audit

Snapshot des aktuellen Zustands + Delta zum Oekosystem.

## Was wird geprueft

1. **Installierte Plugins** - aus settings.json enabledPlugins
2. **Aktive MCP Server** - aus settings.json mcpServers + claude mcp list
3. **Ruflo Tool-Count** - ruflo mcp tools, welche Kategorien aktiv
4. **Vergleich mit Oekosystem** - was existiert, was fehlt, was veraltet

## Ausgabe-Format

CLAUDE SKILL AUDIT - [Datum]

INSTALLIERT:
Plugins:  5 aktiv
MCP:      3 Server (1 connected, 2 auth pending)
Ruflo:    254 Tools

LUECKEN (empfohlen, nicht installiert):
- [Skill/Tool] - [Kategorie] - [Mehrwert]

UPDATES VERFUEGBAR:
- [Plugin] - v1.x nach v2.x

EMPFEHLUNG:
[Eine konkrete Handlung]

## Trigger

/claude-skill-audit
