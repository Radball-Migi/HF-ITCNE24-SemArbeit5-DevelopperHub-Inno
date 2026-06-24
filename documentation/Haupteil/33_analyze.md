---
layout: default
title: 3.3 Analysieren
parent: 3. Hauptteil
nav_order: 6
---
# Analysieren (Analyze) Phase

Die Analyze-Phase ist der dritte Schritt in einem Six Sigma Projekt. Hier werden die in der [Measure-Phase](./32_measure.md) gesammelten Daten analysiert, um die Ursachen von Problemen zu identifizieren. Ziel ist es, die Hauptursachen für Prozessabweichungen zu bestimmen und Hypothesen für Verbesserungen zu entwickeln. Dies umfasst die Nutzung statistischer Methoden und Werkzeuge, um Muster und Zusammenhänge in den Daten zu erkennen.


![Analyze](../../ressources/images/analyze.png)

[Quelle](../Quellverzeichnis/index.md#analyze-phase)

## Zusammenfassung der Datenerhebung

Die Measure-Phase hat gezeigt, dass bestehende Softwareprojekte und Semesterarbeiten aktuell dezentral in verschiedenen Repositories verwaltet werden. Dokumentationen, Quellcode und technische Informationen sind über unterschiedliche Plattformen verteilt und folgen keinen einheitlichen Standards.

Dadurch entsteht ein erhöhter Aufwand bei der Suche nach bestehenden Lösungen, der Wiederverwendung von Projekten sowie beim Wissensaustausch zwischen Entwicklern. Die folgenden Abschnitte analysieren diese Schwachstellen und leiten daraus Anforderungen an eine mögliche Lösung ab.

---

### Fehlende zentrale Übersicht

Aktuell existiert keine zentrale Plattform, welche alle vorhandenen Projekte, Dokumentationen und Entwicklerressourcen zusammenführt.

**Ursachen:**

- Historisch gewachsene Repository-Landschaft
- Unterschiedliche Projektstrukturen
- Fehlende zentrale Katalogisierung
- Dokumentationen sind projektbezogen organisiert

**Auswirkungen:**

- Erschwerte Orientierung innerhalb der Projektlandschaft
- Höherer Aufwand bei der Informationsbeschaffung
- Eingeschränkte Transparenz über vorhandene Arbeiten

Kurz gesagt: **Die vorhandenen Informationen sind verteilt und nur bedingt auffindbar.**

---

### Eingeschränkte Wiederverwendbarkeit

Obwohl bereits zahlreiche Projekte umgesetzt wurden, können deren Ergebnisse nur eingeschränkt für neue Vorhaben genutzt werden.

**Ursachen:**

- Fehlende Such- und Filtermöglichkeiten
- Unterschiedliche Dokumentationsqualität
- Keine zentrale Darstellung von Projekten und deren Beziehungen

**Auswirkungen:**

- Doppelarbeit bei ähnlichen Problemstellungen
- Erhöhter Einarbeitungsaufwand
- Ineffiziente Nutzung bestehender Ressourcen

Oder anders formuliert: **Wissen ist vorhanden, wird jedoch nicht optimal nutzbar gemacht.**

---

### Fehlende Standardisierung

Projekte werden individuell dokumentiert und organisiert. Dadurch entstehen Unterschiede in Aufbau, Struktur und Informationsgehalt.

**Ursachen:**

- Keine verbindlichen Vorgaben
- Unterschiedliche Projektanforderungen
- Fehlende zentrale Plattform mit einheitlichen Standards

**Auswirkungen:**

- Unterschiedliche Benutzererfahrung
- Erschwerte Navigation zwischen Projekten
- Höherer Aufwand bei Wartung und Weiterentwicklung

---

### Anforderungen an Sicherheit und Zugriffsschutz

Da die Plattform teilweise persönliche, schulische oder projektspezifische Inhalte bereitstellen soll, müssen Sicherheitsaspekte bereits bei der Lösungswahl berücksichtigt werden.

**Ursachen:**

- Nicht alle Inhalte sind öffentlich zugänglich
- Unterschiedliche Schutzbedürfnisse der Projekte
- Zentrale Bereitstellung erhöht die Anforderungen an Zugriffskontrollen

**Auswirkungen:**

- Anforderungen an Authentifizierung und Autorisierung
- Berücksichtigung von Datenschutzaspekten
- Notwendigkeit eines geeigneten Berechtigungskonzepts

---

## Evaluation möglicher Developer-Hub-Lösungen

Zur Behebung der identifizierten Schwachstellen wurde eine strukturierte Evaluation verschiedener Developer-Hub-Plattformen durchgeführt. Ziel war es, eine Lösung zu identifizieren, welche die bestehenden Repositories zentral bündeln und gleichzeitig die technischen sowie organisatorischen Anforderungen erfüllt.

Die Evaluation erfolgte in zwei Schritten:

1. Grob-Evaluation zur Eingrenzung geeigneter Produkte
2. Detail-Evaluation anhand definierter Bewertungskriterien

Im Rahmen der Marktanalyse wurden verschiedene Lösungen untersucht, darunter Backstage, Red Hat Developer Hub (RHDH), Port, Cortex, OpsLevel, Atlassian Compass und Harness Internal Developer Portal.

Nach Anwendung der definierten Ausschluss- und Auswahlkriterien wurden die folgenden Plattformen für die Detailanalyse ausgewählt:

- Backstage
- Red Hat Developer Hub (RHDH)
- Port

### Ergebnis der Evaluation

Die Bewertung erfolgte anhand technischer und organisatorischer Kriterien wie Kubernetes-Integration, Self-Hosting, Erweiterbarkeit, Benutzerfreundlichkeit, Community-Unterstützung, Betriebsaufwand und Kosten.

Die gewichtete Gesamtbewertung ergab, dass Backstage die definierten Anforderungen am besten erfüllt und die höchste Gesamtpunktzahl erreicht.

> **Hinweis:** Die vollständige Evaluation inklusive Marktanalyse, Bewertungsmatrix, Gewichtungsmodell und Entscheidungsgrundlage ist im Kapitel [Evaluation Developer Hubs](../../ressources/docs/Evaluation.md) dokumentiert.

---

## Erkenntnisse der Analyse

Die Analyse zeigt, dass die identifizierten Herausforderungen primär auf das Fehlen einer zentralen Plattform für Entwicklerressourcen zurückzuführen sind.

Die durchgeführte Evaluation verschiedener Developer-Hub-Lösungen hat bestätigt, dass geeignete Plattformen existieren, um diese Herausforderungen zu adressieren. Insbesondere Backstage erfüllt die Anforderungen hinsichtlich Kubernetes-Integration, Erweiterbarkeit, Self-Hosting und Zukunftssicherheit am umfassendsten.

Auf Basis dieser Erkenntnisse wird Backstage als Zielplattform für die Umsetzung des Proof of Concepts ausgewählt.

---

## Wie könnte dies gelöst werden?

Aus der Analyse lassen sich folgende Lösungsansätze ableiten:

- Einführung eines zentralen Developer Hubs auf Basis von Backstage
- Aufbau einer Kubernetes-basierten Betriebsumgebung
- Integration bestehender Software-Repositories
- Einführung eines zentralen Software-Katalogs
- Standardisierte Darstellung von Projekten und Dokumentationen
- Implementierung eines geeigneten Authentifizierungs- und Berechtigungskonzepts
- Schaffung einer zentralen Wissens- und Entwicklerplattform

Diese Ansätze werden in der **Improve-Phase** konkretisiert, umgesetzt und anhand eines Proof of Concepts technisch validiert.