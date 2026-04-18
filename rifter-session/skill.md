---
name: rifter-session
description: Vollständiges Rifter Session-Startprotokoll — MCP-Status, Ruflo-Tools, Memory-Index, aktive Projekte, GCP-Health in einem Befehl.
category: automation
version: 0.1.0
status: stub
---

# rifter-session

<!-- STUB — Implementierung ausstehend -->

Ersetzt das manuelle Session-Start-Ritual. Führt aus:

1. `claude mcp list` → MCP-Status
2. `ruflo mcp tools` → Tool-Count
3. Memory MEMORY.md laden → Projekt-Übersicht
4. GCP `/health/full` → RIFTERBOT-Status
5. Gibt Session-Status-Protokoll im Standard-Format aus

## Trigger

```
/rifter-session
```
