---
layout: default
title: 5.1 Erreichte Ziele
parent: 5. Abschluss
nav_order: 3
---

# Wurden sämtliche Zielsetzungen erfüllt?



![Reached Goals](../../ressources/images/reached-goals.png)

[Quelle](../Quellverzeichnis/index.md#erreichte-ziele) 


Zu Beginn der Semesterarbeit wurden die Projektziele bewusst offen formuliert. Dadurch blieb während der Umsetzung genügend Spielraum, um auf neue Erkenntnisse sowie technische und organisatorische Herausforderungen reagieren zu können. Gleichzeitig bildeten die definierten Ziele einen klaren Rahmen für die Konzeption, Umsetzung und Bewertung des entwickelten Proof of Concept.

Die Zielerreichung wird nachfolgend anhand der ursprünglich definierten Projektziele bewertet.

| Zielsetzung | Kurzbeschreibung | Erfüllungsgrad |
|-------------|------------------|----------------|
| Aufbau und Bereitstellung eines Kubernetes-Clusters | Aufbau einer stabilen Kubernetes-Umgebung als Grundlage für den Betrieb des Developer Hubs. | ✅ |
| Evaluation und Auswahl eines geeigneten Developer Hubs | Vergleich verschiedener Lösungen und Auswahl einer geeigneten Plattform anhand definierter Kriterien. | ✅ |
| Implementierung und Deployment des Developer Hubs | Bereitstellung und Konfiguration von Backstage innerhalb des Kubernetes-Clusters. | ✅ |
| Integration und zentrale Verwaltung von Software-Repositories | Integration bestehender Semesterprojekte sowie zentrale Bereitstellung von Dokumentation und Metadaten. | ✅ |
| Dokumentation sowie konzeptionelle KI-Evaluierung | Vollständige Projektdokumentation sowie optionale Betrachtung möglicher KI-Erweiterungen. | ⚠️ |

Die Bewertung erfolgte sowohl anhand der technischen Umsetzung als auch unter Berücksichtigung der im Projekt gewonnenen organisatorischen und architektonischen Erkenntnisse.

Im Folgenden wird erläutert, wie die einzelnen Ziele erreicht wurden und welche Erkenntnisse sich daraus ergeben haben.

---

## Aufbau und Bereitstellung eines Kubernetes-Clusters

Zu Beginn der Semesterarbeit wurde ein lokaler Kubernetes-Cluster aufgebaut, welcher als technische Grundlage für den späteren Betrieb des Developer Hubs diente. Innerhalb dieser Umgebung konnten sämtliche benötigten Kubernetes-Ressourcen erfolgreich bereitgestellt und Backstage stabil betrieben werden.

Der Cluster bildete während der gesamten Umsetzung eine reproduzierbare Entwicklungs- und Testumgebung und erfüllte damit die definierten Anforderungen.

✅ **Ziel erreicht**

---

## Evaluation und Auswahl eines geeigneten Developer Hubs

Ein wesentlicher Bestandteil der Arbeit war die Evaluation verschiedener Developer-Hub-Lösungen. Hierfür wurden mehrere Produkte anhand definierter Bewertungskriterien wie Funktionalität, Erweiterbarkeit, Integrationsfähigkeit, Benutzerfreundlichkeit sowie Implementierungsaufwand untersucht.

Auf Grundlage dieser Evaluation wurde Backstage als geeignetste Plattform ausgewählt und anschliessend praktisch umgesetzt.

Die vorgängige Evaluation erwies sich als sinnvoll und bildete eine fundierte Entscheidungsgrundlage für die anschliessende Implementierung.

✅ **Ziel erreicht**

---

## Implementierung und Deployment des Developer Hubs

Nach Abschluss der Evaluation wurde Backstage innerhalb des Kubernetes-Clusters implementiert und konfiguriert. Neben der eigentlichen Bereitstellung wurden die benötigten Plugins integriert sowie die Plattform für den praktischen Einsatz vorbereitet.

Der entwickelte Proof of Concept zeigt, dass Backstage erfolgreich innerhalb einer Kubernetes-Umgebung betrieben werden kann und als zentrale Plattform für Entwicklerressourcen genutzt werden kann.

Damit konnte das definierte Projektziel vollständig erreicht werden.

✅ **Ziel erreicht**

---

## Integration und zentrale Verwaltung von Software-Repositories

Ein zentrales Ziel der Semesterarbeit bestand in der Integration bestehender Softwareprojekte innerhalb des Developer Hubs.

Hierfür wurden die Semesterprojekte aus dem zweiten bis fünften Semester erfolgreich integriert und mit den notwendigen Metadaten ergänzt. Zusätzlich wurden TechDocs eingerichtet und die Projekte im Software Catalog kategorisiert.

Dadurch entstand eine zentrale Übersicht der vorhandenen Softwareprojekte, welche den Zugriff auf Quellcode, Dokumentationen sowie weitere Projektinformationen deutlich vereinfacht.

Während der Umsetzung zeigte sich jedoch auch, dass die Integration bestehender Projekte einen erheblichen Standardisierungsaufwand erfordert. Unterschiedliche Repository-Strukturen mussten vereinheitlicht und um zusätzliche Metadaten ergänzt werden, bevor eine vollständige Integration möglich war.

Das technische Projektziel konnte vollständig erreicht werden. Gleichzeitig wurde deutlich, dass eine produktive Einführung innerhalb eines Unternehmens umfangreiche organisatorische Anpassungen erfordern würde.

✅ **Ziel erreicht**

---

## Dokumentation sowie konzeptionelle KI-Evaluierung

Die Umsetzung des Projekts wurde während der gesamten Semesterarbeit fortlaufend dokumentiert. Sämtliche Projektphasen, Architekturentscheidungen sowie die technische Umsetzung wurden nachvollziehbar beschrieben und bilden den Hauptbestandteil dieser Arbeit.

Die ursprünglich geplante konzeptionelle Betrachtung möglicher KI-Erweiterungen konnte hingegen nicht mehr umgesetzt werden. Während der praktischen Umsetzung zeigte sich, dass insbesondere die Integration der bestehenden Software-Repositories sowie die Konfiguration von Backstage deutlich mehr Zeit in Anspruch nahmen als ursprünglich geplant. Um den Fokus auf die erfolgreiche Umsetzung des Proof of Concept zu legen, wurde entschieden, die optionale KI-Evaluierung zugunsten der Kernziele des Projekts zurückzustellen.

Da die KI-Thematik bereits zu Projektbeginn als optionale Erweiterung definiert wurde, stellt dies keine Zielverfehlung dar, sondern eine bewusste Priorisierung innerhalb des verfügbaren Projektumfangs.

⚠️ **Ziel teilweise erreicht**

---

## Gesamtbewertung der Zielerreichung

Die wesentlichen Projektziele der Semesterarbeit konnten erfolgreich erreicht werden. Der entwickelte Proof of Concept bestätigt die technische Machbarkeit eines Kubernetes-basierten Developer Hubs auf Basis von Backstage und zeigt, dass bestehende Software-Repositories erfolgreich zentral verwaltet und dokumentiert werden können.

Die optionale KI-Evaluierung wurde aufgrund des zeitlichen Projektumfangs nicht umgesetzt. Während der praktischen Arbeiten zeigte sich, dass insbesondere die Integration der bestehenden Repositories sowie die Konfiguration der Plattform einen höheren Aufwand verursachten als ursprünglich erwartet. Da die KI-Evaluierung nicht Bestandteil der Kernfunktionalität des Proof of Concept war, wurde sie zugunsten der erfolgreichen Umsetzung der Hauptziele bewusst zurückgestellt.

Darüber hinaus führte die praktische Umsetzung zu einer wichtigen zusätzlichen Erkenntnis. Während die technische Implementierung erfolgreich realisiert werden konnte, zeigte sich, dass der eigentliche Aufwand einer produktiven Einführung nicht in der Bereitstellung der Plattform liegt, sondern in der notwendigen Standardisierung bestehender Softwareprojekte sowie der Anpassung organisatorischer Prozesse.

Die daraus gewonnenen Erkenntnisse bilden eine fundierte Grundlage für die Bewertung einer möglichen Einführung eines Developer Hubs innerhalb der ISE AG. Der entwickelte Proof of Concept konnte somit nicht nur die technische Machbarkeit nachweisen, sondern gleichzeitig die Chancen und Herausforderungen einer produktiven Einführung transparent aufzeigen. Dadurch erfüllt die Semesterarbeit ihren ursprünglichen Zweck und liefert eine belastbare Entscheidungsgrundlage für zukünftige Vorhaben im Bereich zentralisierter Entwicklerplattformen.