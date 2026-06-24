---
layout: default
title: 3.1 Definieren
parent: 3. Hauptteil
nav_order: 4
---
# Definieren (Define) Phase

Die Define-Phase ist der erste Schritt in einem Six Sigma Projekt. In dieser Phase wird das Projekt klar definiert, um sicherzustellen, dass alle Beteiligten ein gemeinsames Verständnis der Ziele und des Umfangs haben. Ein wesentlicher Bestandteil dieser Phase ist die Identifizierung und Beschreibung des zu lösenden Problems oder der zu verbessernden Prozesse.

![Define](../../ressources/images/define.png)

[Quelle](../Quellverzeichnis/index.md#define-phase)

## Zielvorstellung

Am Ende der Semesterarbeit soll ein Kubernetes-basierter Developer Hub als zentraler Einstiegspunkt für bestehende Softwareprojekte und Entwicklerressourcen bereitgestellt werden. Die Plattform soll eine strukturierte und einheitliche Übersicht über vorhandene Repositories ermöglichen und den Zugriff auf Projektdokumentationen, Quellcode-Repositories sowie weitere relevante Informationen vereinfachen.

Im Rahmen eines Proof of Concepts (PoC) werden verschiedene Developer-Hub-Lösungen evaluiert und anhand definierter Kriterien miteinander verglichen. Die ausgewählte Plattform soll anschliessend in einer Kubernetes-Umgebung implementiert und konfiguriert werden.

Ein weiterer Schwerpunkt liegt auf der Integration bestehender Software-Repositories in den Developer Hub. Dadurch sollen bisher dezentral verwaltete Projekte zentral gebündelt und deren Wiederverwendbarkeit verbessert werden. Gleichzeitig soll sichergestellt werden, dass nur berechtigte Benutzer auf die bereitgestellten Inhalte zugreifen können.

Die Lösung soll praxisnah umgesetzt, nachvollziehbar dokumentiert und so gestaltet werden, dass sie als Grundlage für zukünftige Developer-Hub- oder Wissensmanagement-Plattformen dienen kann.

---

## Ressourceneinsatz

Für die Umsetzung der Semesterarbeit stehen folgende Ressourcen und Werkzeuge zur Verfügung:

- **Kubernetes-Umgebung**
    Bereitstellung und Betrieb des Developer Hubs innerhalb einer containerisierten Plattform.

- **Docker / Container-Technologien**
    Containerisierung und Bereitstellung der ausgewählten Developer-Hub-Lösung.

- **Developer-Hub-Plattformen**
    Evaluation verschiedener Lösungen wie beispielsweise Backstage, Port oder Open-Source-Alternativen.

- **GitHub Repository**
    Versionsverwaltung, Projektorganisation, Dokumentation und Verwaltung der Software-Repositories.

- **Visual Studio Code**
    Entwicklungsumgebung für Konfigurationen, Dokumentation und Infrastrukturdefinitionen.

- **GitHub Pages / MkDocs**
    Erstellung und Bereitstellung der Projektdokumentation.

- **Vorhandene Software-Repositories**
    Bestehende Semesterarbeiten und Entwicklungsprojekte als Grundlage für die Integration in den Developer Hub.


---

## Warum wird die Zielvorstellung aktuell nicht erreicht?

Im Verlauf der Ausbildung und verschiedener Projekte wurden zahlreiche Softwarelösungen und Semesterarbeiten erstellt. Diese befinden sich aktuell in unterschiedlichen Repositories und sind dezentral organisiert. Dokumentationsstandards und Projektstrukturen unterscheiden sich teilweise erheblich, wodurch eine zentrale Übersicht über bestehende Arbeiten fehlt.

Diese Situation führt zu mehreren Einschränkungen:
- Vorhandene Projekte sind nur eingeschränkt auffindbar.
- Die Wiederverwendung bestehender Lösungen wird erschwert.
- Wissen verteilt sich auf mehrere Repositories und Dokumentationsquellen.
- Neue Entwickler oder Interessierte erhalten keinen zentralen Einstiegspunkt in die vorhandene Projektlandschaft.
- Informationen zu Projekten müssen manuell gesucht und zusammengetragen werden.

Um die angestrebte Zielvorstellung zu erreichen, sind daher folgende technische und organisatorische Massnahmen erforderlich:
- Evaluation geeigneter **Developer-Hub-Plattformen**
- Definition von **Auswahl- und Bewertungskriterien**
- Aufbau einer **Kubernetes-basierten Laufzeitumgebung**
- Integration bestehender **Software-Repositories**
- Konzeption eines geeigneten **Zugriffs- und Berechtigungskonzepts**
- Strukturierte Dokumentation der Architektur, Evaluation und Implementierung

Diese Massnahmen sind notwendig, um eine zentrale Plattform für Entwicklerressourcen zu schaffen, die Auffindbarkeit bestehender Projekte zu verbessern und den Wissensaustausch nachhaltig zu fördern.