---
name: rifter-brain-eval
description: Manueller Brain-Eval-Trigger — ruft ClaudeBrain.evaluate_daily() außerhalb des 06:00-UTC-Zyklus auf. Für ad-hoc Markt-Analyse und Signal-Check.
category: finance
version: 0.1.0
status: stub
---

# rifter-brain-eval

<!-- STUB — Implementierung ausstehend -->

Wenn dieser Skill aufgerufen wird:

1. POST `/brain/evaluate` auf GCP-Server
2. Gibt Recommendations-JSON zurück
3. Formatiert SCALP/SWING-Signals als Tabelle
4. Zeigt Konfidenz, Narrative-Trigger, Qualitätskriterien

## Trigger

```
/rifter-brain-eval
```
