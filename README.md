# Triathlon 70.3 – iPhone Web-App (PWA)

Dies ist eine eigenständige mobile Version des bestehenden Python-Trainingsplans (Stand 23.10.2026).

## Was bereits funktioniert
- Trainingskalender mit den echten Einheiten aus `training_plan.csv` (inkl. Schwimmen Mo/Di/Do)
- Details, Distanzen, Intervalle, Soll-Dauer und Zielvorgaben
- Einheiten abhaken; lokale Speicherung auf dem jeweiligen Gerät
- Fortschrittsanzeige, CSV-Import eines neu erzeugten Trainingsplans, Export der Häkchen
- Offline-Zugriff nach erstmaligem Laden auf HTTPS-Hosting (Service Worker)

## iPhone installieren
Eine PWA muss für die Installation über eine **HTTPS-Webadresse** erreichbar sein. Lade **den Inhalt dieses Ordners** in ein privates/geeignetes HTTPS-Webhosting (z.B. GitHub Pages; Vorsicht: öffentliche GitHub-Pages-Seiten veröffentlichen auch die Trainingsplan-CSV). Öffne dann die URL in **Safari auf dem iPhone**, tippe auf **Teilen → Zum Home-Bildschirm**.

Du kannst die App vorab am Mac mit `python3 -m http.server 8000` im Projektordner testen und `http://localhost:8000` öffnen. `file://` direkt per Doppelklick ist nicht geeignet.

## Strava-Synchronisierung
**Nicht enthalten:** Automatischer Strava-Import auf dem iPhone, Live-Synchronisierung mit der Mac-App, Übernahme der Mac-Trainingslogs und ein Cloud-Account. Die bestehende Strava-Integration läuft weiterhin in der Python-Mac-App. Für eine sichere mobile Synchronisierung ist ein HTTPS-Backend mit OAuth-Token-Speicherung auf dem Server notwendig. **Niemals Client Secret oder Refresh Token in die öffentlich ausgelieferte Web-App einfügen.**

## Datenhinweis
Häkchen liegen in localStorage auf dem Gerät. Browserdaten-Löschung kann diese entfernen: regelmäßig CSV exportieren. Eine neue Plan-CSV kann in der App importiert werden.
