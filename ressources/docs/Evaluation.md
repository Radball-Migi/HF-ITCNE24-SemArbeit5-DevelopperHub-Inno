# Evaluation Developer Hubs – Punktebewertung

## Legende der Punktebewertung

| Punkte | Bedeutung                      |
| ------ | ------------------------------ |
| 1      | Sehr schlecht / kaum geeignet  |
| 2      | Eingeschränkt geeignet         |
| 3      | Durchschnittlich / ausreichend |
| 4      | Gut geeignet                   |
| 5      | Sehr gut geeignet              |

---

# Bewertungsmatrix

| Kriterium | Gewichtung | Backstage | RHDH | Port |
|---|---|---|---|---|
| Kubernetes Integration | Hoch | 5 | 5 | 3 |
| Self-Hosting | Hoch | 5 | 5 | 2 |
| Erweiterbarkeit | Hoch | 5 | 4 | 3 |
| Benutzerfreundlichkeit | Mittel | 3 | 4 | 5 |
| Dokumentation & Community | Mittel | 5 | 4 | 3 |
| Enterprise-Funktionen | Mittel | 4 | 5 | 4 |
| Betriebsaufwand | Mittel | 3 | 2 | 5 |
| Kosten | Hoch | 5 | 2 | 3 |
| KI-Integration | Mittel | 5 | 4 | 3 |

---

# Gesamtbewertung

| Plattform     | Gesamtpunkte  | Bewertung              |
| ------------- | ------------- | ---------------------- |
| **Backstage** | **40 Punkte** | **Sehr gut geeignet**  |
| RHDH          | **35 Punkte** | Gut geeignet           |
| Port          | **31 Punkte** | Eingeschränkt geeignet |

---

# Kurzbegründung

## Backstage
Backstage bietet die höchste Flexibilität, starke Kubernetes-Integration und sehr gute Erweiterbarkeit. Die Plattform eignet sich besonders gut für die Anforderungen der ISE AG, da zukünftige Erweiterungen sowie KI-Integrationen flexibel umgesetzt werden können.

## Red Hat Developer Hub (RHDH)
RHDH bietet viele Enterprise-Funktionen und professionelle Unterstützung, verursacht jedoch höhere Kosten und zusätzlichen Betriebsaufwand.

## Port
Port überzeugt durch einfache Bedienung und schnellen Einstieg, bietet jedoch weniger Kontrolle und geringere Flexibilität für individuelle Anpassungen.

---

# Hinweis zu Microsoft und Azure

Im Rahmen der Evaluation wurde geprüft, ob Microsoft ein eigenes vollständiges Developer-Hub- oder Internal-Developer-Portal anbietet. Dabei zeigte sich, dass Microsoft aktuell keine eigenständige Plattform vergleichbar mit Backstage oder RHDH bereitstellt.

Microsoft verweist stattdessen auf die Nutzung von Backstage in Kombination mit Azure-Diensten wie:

- Azure Kubernetes Service (AKS)
- Azure DevOps
- GitHub
- Azure AI Services

Dadurch bestätigt sich Backstage zusätzlich als geeignete und zukunftssichere Lösung für moderne Cloud- und Kubernetes-Umgebungen.

## Quellen

- Microsoft Learn – Developer Self-Service Foundation  
  https://learn.microsoft.com/en-us/platform-engineering/developer-self-service

- Backstage Dokumentation – Microsoft / Azure Integration  
  https://backstage.io/docs/integrations/azure/org

- Backstage Microsoft Authentication Provider  
  https://backstage.io/docs/auth/microsoft/provider/