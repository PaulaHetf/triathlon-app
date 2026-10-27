# Triathlon 70.3 – iPhone-App V9

## Neue Funktionen
- Wochenansicht mit Vor/Zurück-Pfeilen und Hervorhebung des heutigen Tages.
- Abgehakte Einheiten verschwinden sofort aus der aktiven Woche und sind im Archiv weiterhin einsehbar und wieder als offen markierbar.
- Vorwochen bleiben im Archiv, auch wenn einzelne Einheiten offen sind.
- Sechs Wettkämpfe 2027 werden beim ersten V9-Start ergänzt, ohne vorhandene Wettkämpfe zu überschreiben.
- Training vom 26.10.2026 bis 17.10.2027: Schwimmen ausschließlich Mo/Di/Do, maximal zwei Radeinheiten pro Woche, 2–3 Läufe, Krafttraining und ein Ruhetag; progressiv wechselnde kurze und längere Rad- und Laufintervalle, Entlastungs- und Wettkampfwochen. Die konkreten Einheiten stehen in `training_plan.csv`.
- Backup/Restore (.json) unter **Daten** für Häkchen, Wettkämpfe, Verschiebungen, FTP und optional importierten Trainingsplan.

## Aktualisieren
Die sechs Dateien direkt ins Stammverzeichnis des GitHub-Pages-Repositories hochladen und vorhandene Dateien ersetzen. Keine Ordnerstruktur ändern. **Vor einem Update nach Möglichkeit bisherige Häkchen und Wettkämpfe exportieren.** Die App verwendet weiterhin dieselben lokalen Schlüssel für Häkchen (`triathlon_mobile_records_v1`), Wettkämpfe (`triathlon_mobile_races_v1`) und Verschiebungen (`triathlon_mobile_moves_v5`).

## Grenzen
Lokaler Browser-/PWA-Speicher ist keine dauerhafte Cloud-Sicherung. Installierte iPhone-PWA und Safari können unterschiedliche lokale Speicher besitzen. Backup auf dem iPhone regelmäßig sichern. Ein von Hand importierter Plan ersetzt den mitgelieferten V9-Plan, bis die Import-Daten entfernt oder ein Backup ohne eigenen Plan wiederhergestellt wird. Die Wettkampfanpassungen sind regelbasiert und keine individualisierte Trainingsdiagnostik. Keine automatische Strava-Synchronisierung.
