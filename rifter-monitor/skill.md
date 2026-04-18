---
name: rifter-monitor
description: RIFTERBOT Live-Status — lädt /health/full vom GCP-Server, zeigt Balance, offene Positionen, Guardian-Status und letzte Logs. Kein SSH nötig.
category: automation
version: 0.1.0
status: stub
---

# rifter-monitor

<!-- STUB — Implementierung ausstehend -->

Wenn dieser Skill aufgerufen wird:

1. Verbinde mit GCP `rifterbot` (104.198.252.28:8088)
2. GET `/health/full` → parse JSON
3. Zeige: Status, Balance USDT, offene Positions, Guardian-Level, letzte Errors
4. Telegram-Alert wenn Balance < $150 oder Status != "ok"

## Trigger

```
/rifter-monitor
```

## Ausgabe-Format

```
RIFTER LIVE — [timestamp]
Status: ok | Balance: $XXX | Pos: X open
Guardian: [level] | Brain: [last_eval]
```
