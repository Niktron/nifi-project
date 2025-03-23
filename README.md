# Apache NiFi Project

Dieses Repository enthält eine Docker-basierte Implementierung von Apache NiFi sowie Übungsbeispiele, die die grundlegenden und erweiterten Funktionen der Plattform veranschaulichen. Apache NiFi ist eine leistungsstarke Plattform zur Automatisierung und Verwaltung von Datenflüssen, die einfach zu installieren und flexibel zu konfigurieren ist.

## Ordnerstruktur

- **[./docker](./docker)**  
  Enthält alle notwendigen Dateien und Konfigurationen für die Docker-basierte Bereitstellung von Apache NiFi. Darunter:
  - `docker-compose.yaml`: Definition der Multi-Container-Umgebung.
  - `conf/`: Konfigurationsdateien für Nginx und andere Services.
  - `.env`: Environment-Variablen zur einfachen Anpassung der Cluster-Konfiguration.

- **[./examples](./examples)**  
  Übungsbeispiele zur Veranschaulichung der NiFi-Funktionalität. Darunter direkte NiFi Templates zum importieren von Flows und ausprobieren, als auch andere Dateien.
  - **[move_files](./examples/move_files)**: Beinhaltet Template Lösung.
  - **[department_router](./examples/department_router)**: Beinhaltet Template Lösungen und andere Dateien.

- **[./docs](./docs)**  
  Enthält Dokumentationen und weiterführende Anleitungen zur Installation, Konfiguration und Nutzung von Apache NiFi. Auch das PDF mit der vollständigen Hausarbeit und den Übungsbeschreibungen ist hier abgelegt.

## Quickstart

1. **Voraussetzungen**  
   - Docker und Docker Compose müssen installiert sein.  
   - Mindestanforderungen an RAM und CPU sind abhängig von der Größe und Komplexität der Workflows.

2. **Bereitstellung**  
   Führe den folgenden Command im Ordner `docker` aus:  
   ```bash
   docker compose up -d
   ```
   Der Cluster wird gestartet und ist über [http://localhost](http://localhost) erreichbar.

3. **Übungen durchführen**  
   Die Übungsworkflows können mithilfe der bereitgestellten Beispiele unter `./examples` in der NiFi-Benutzeroberfläche nachgebaut und getestet werden.

## Lizenz

Dieses Projekt steht unter der **MIT License**. Details findest du in der Datei [LICENSE](./LICENSE).
