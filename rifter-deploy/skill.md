---
name: rifter-deploy
description: RIFTERBOT Deploy-Pipeline — SCP Datei zu GCP, Restart, Health-Check, Verifikation in einem Befehl. Kein manuelles SSH nötig.
category: automation
version: 0.1.0
status: stub
---

# rifter-deploy

<!-- STUB — Implementierung ausstehend -->

Wenn dieser Skill mit Dateipfad aufgerufen wird:

1. `gcloud compute scp [datei] rifterbot:/home/peter/backend/...`
2. datetime-Fix in main.py prüfen (falls main.py deployed)
3. `sudo systemctl restart rifterbot`
4. `sleep 8` → `/health/full` → Status ausgeben

## Trigger

```
/rifter-deploy [datei]
```

## Beispiel

```
/rifter-deploy backend/organism/capital_rotator.py
```
