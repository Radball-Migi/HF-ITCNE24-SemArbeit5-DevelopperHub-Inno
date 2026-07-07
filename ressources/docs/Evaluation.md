# Evaluation Developer Hubs

## Vorgehen

Die Evaluation erfolgte in zwei Schritten:

1. **Grob-Evaluation** zur Eingrenzung des Marktes und Auswahl geeigneter Kandidaten.
2. **Detail-Evaluation** der ausgewählten Lösungen anhand definierter Bewertungskriterien.

Dadurch konnte der Umfang der Analyse auf die für die Anforderungen der ISE AG relevantesten Produkte reduziert werden.

---

# Grob-Evaluation

## Marktanalyse

Im Rahmen einer ersten Recherche wurden verschiedene Developer-Hub- und Internal-Developer-Portal-Lösungen untersucht.

Dabei wurden unter anderem folgende Produkte betrachtet:

- Backstage
- Red Hat Developer Hub (RHDH)
- Port
- Cortex
- OpsLevel
- Atlassian Compass
- Harness Internal Developer Portal

Da der Umfang der Semesterarbeit eine detaillierte Analyse aller verfügbaren Lösungen nicht zulässt, wurde eine Grob-Evaluation durchgeführt.

---

## Kriterien der Grob-Evaluation

Für die Eingrenzung wurden folgende Ausschluss- und Auswahlkriterien definiert:

| Kriterium                            | Begründung                                               |
| ------------------------------------ | -------------------------------------------------------- |
| Kubernetes-Unterstützung             | Die Zielplattform basiert auf Kubernetes                 |
| Self-Hosting möglich                 | Betrieb soll lokal bzw. unter eigener Kontrolle erfolgen |
| Aktive Weiterentwicklung             | Langfristige Zukunftssicherheit                          |
| Marktverbreitung                     | Relevanz und Akzeptanz in Unternehmen                    |
| Dokumentation verfügbar              | Nachvollziehbarkeit und Implementierbarkeit              |
| Unterstützung von Software-Katalogen | Zentrale Verwaltung von Projekten und Services           |
| Erweiterbarkeit                      | Möglichkeit für spätere Integrationen (z. B. KI)         |

---

## Ergebnis der Grob-Evaluation

| Produkt                      | Ergebnis                | Begründung                                                                      |
| ---------------------------- | ----------------------- | ------------------------------------------------------------------------------- |
| Backstage                    | Ausgewählt              | Hohe Verbreitung, Kubernetes-Fokus, Self-Hosting und grosse Erweiterbarkeit     |
| Red Hat Developer Hub (RHDH) | Ausgewählt              | Enterprise-Variante von Backstage mit professionellem Support                   |
| Port                         | Ausgewählt              | Etablierte Developer-Portal-Lösung mit moderner Benutzeroberfläche              |
| Cortex                       | Nicht weiter betrachtet | Fokus auf grosse Enterprise-Organisationen, eingeschränkte Relevanz für den PoC |
| OpsLevel                     | Nicht weiter betrachtet | Fokus auf SaaS-Betrieb, Self-Hosting nicht im Vordergrund                       |
| Atlassian Compass            | Nicht weiter betrachtet | Starke Abhängigkeit vom Atlassian-Ökosystem                                     |
| Harness IDP                  | Nicht weiter betrachtet | Starke Ausrichtung auf bestehende Harness-Kunden                                |

---

## Auswahl der Detail-Evaluation

Auf Basis der Grob-Evaluation wurden folgende Lösungen für die Detailanalyse ausgewählt:

- Backstage
- Red Hat Developer Hub (RHDH)
- Port

Diese Produkte erfüllen die technischen Anforderungen der ISE AG am besten und repräsentieren gleichzeitig unterschiedliche Ansätze:

- Backstage als Open-Source-Referenz und Marktstandard
- RHDH als Enterprise-Lösung
- Port als SaaS-orientierte Plattform

---

# Detail-Evaluation

## Legende der Punktebewertung

|Punkte|Bedeutung|
|---|---|
|1|Sehr schlecht / kaum geeignet|
|2|Eingeschränkt geeignet|
|3|Durchschnittlich / ausreichend|
|4|Gut geeignet|
|5|Sehr gut geeignet|

---

## Gewichtungsmodell

|Gewichtung|Faktor|
|---|---|
|Hoch|3|
|Mittel|2|
|Niedrig|1|

---

## Bewertungsmatrix

| Kriterium                 | Gewichtung | Faktor | Backstage | RHDH | Port |
| ------------------------- | ---------- | ------ | --------- | ---- | ---- |
| Kubernetes Integration    | Hoch       | 3      | 5         | 5    | 3    |
| Self-Hosting              | Hoch       | 3      | 5         | 5    | 2    |
| Erweiterbarkeit           | Hoch       | 3      | 5         | 4    | 3    |
| Benutzerfreundlichkeit    | Mittel     | 2      | 3         | 4    | 5    |
| Dokumentation & Community | Mittel     | 2      | 5         | 4    | 3    |
| Enterprise-Funktionen     | Mittel     | 2      | 4         | 5    | 4    |
| Betriebsaufwand           | Mittel     | 2      | 3         | 2    | 5    |
| Kosten                    | Hoch       | 3      | 5         | 2    | 3    |
| KI-Integration            | Mittel     | 2      | 5         | 4    | 3    |

---

## Gewichtete Gesamtbewertung

|Kriterium|Faktor|Backstage|RHDH|Port|
|---|---|---|---|---|
|Kubernetes Integration|3|15|15|9|
|Self-Hosting|3|15|15|6|
|Erweiterbarkeit|3|15|12|9|
|Benutzerfreundlichkeit|2|6|8|10|
|Dokumentation & Community|2|10|8|6|
|Enterprise-Funktionen|2|8|10|8|
|Betriebsaufwand|2|6|4|10|
|Kosten|3|15|6|9|
|KI-Integration|2|10|8|6|
|**Total**||**100**|**86**|**73**|

---

# Ergebnis

| Plattform                        | Gesamtpunkte   | Bewertung             |
| -------------------------------- | -------------- | --------------------- |
| **Backstage**                    | **100 Punkte** | **Sehr gut geeignet** |
| **Red Hat Developer Hub (RHDH)** | **86 Punkte**  | Gut geeignet          |
| **Port**                         | **73 Punkte**  | Geeignet              |

---

# Kurzbegründung

## Backstage

Backstage bietet die höchste Flexibilität, eine sehr gute Kubernetes-Integration sowie umfangreiche Erweiterungsmöglichkeiten. Die Plattform erfüllt die Anforderungen der ISE AG am besten und ermöglicht zukünftige Erweiterungen wie KI-gestützte Funktionen oder zusätzliche Integrationen.

## Red Hat Developer Hub (RHDH)

RHDH bietet professionelle Enterprise-Funktionen und Supportmöglichkeiten. Die Plattform verursacht jedoch höhere Kosten und einen grösseren Betriebsaufwand als Backstage.

## Port

Port überzeugt durch Benutzerfreundlichkeit und einen schnellen Einstieg. Die Plattform bietet jedoch weniger Kontrolle über die Infrastruktur und geringere Anpassungsmöglichkeiten.

---

# Abgrenzung Microsoft-Lösungen

Im Rahmen der Marktanalyse wurde geprüft, ob Microsoft ein eigenes vollständiges Developer-Hub- oder Internal-Developer-Portal anbietet.

Dabei zeigte sich, dass Microsoft aktuell keine eigenständige Plattform vergleichbar mit Backstage, RHDH oder Port bereitstellt.

Microsoft empfiehlt stattdessen die Nutzung von Backstage in Kombination mit Azure-Diensten wie:

- Azure Kubernetes Service (AKS)
- Azure DevOps
- GitHub
- Azure AI Services

Dadurch bestätigt sich Backstage zusätzlich als geeignete und zukunftssichere Lösung für moderne Cloud- und Kubernetes-Umgebungen.

## Quellen

- Microsoft Learn – Developer Self-Service Foundation  
    [https://learn.microsoft.com/en-us/platform-engineering/developer-self-service](https://learn.microsoft.com/en-us/platform-engineering/developer-self-service)
    
- Backstage Dokumentation – Azure Integration  
    [https://backstage.io/docs/integrations/azure/org](https://backstage.io/docs/integrations/azure/org)
    
- Backstage Microsoft Authentication Provider  
    [https://backstage.io/docs/auth/microsoft/provider/](https://backstage.io/docs/auth/microsoft/provider/)
    

---

# Entscheid

Für die Umsetzung des Developer Hubs bei der ISE AG wird **Backstage** ausgewählt.

## Begründung

Backstage erreicht die höchste Gesamtbewertung und bietet die beste Kombination aus:

- Kubernetes-Integration
- Self-Hosting
- Erweiterbarkeit
- Zukunftssicherheit
- Community-Unterstützung
- KI-Integrationsmöglichkeiten

Die Plattform erfüllt die technischen und organisatorischen Anforderungen der ISE AG am umfassendsten und bietet gleichzeitig die grösste Flexibilität für zukünftige Erweiterungen.