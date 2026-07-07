# Deployment Steps: Backstage PoC

Dieses Dokument beschreibt die Deployment-Schritte für Issue #5: `infra: Deploy Backstage on Kubernetes`.

## Ziel

Backstage soll als Proof of Concept in Kubernetes bereitgestellt werden. Dabei werden die Kubernetes-Ressourcen versioniert und über Kustomize ausgerollt.

## Voraussetzungen

- Kubernetes-Cluster ist verfügbar
- `kubectl` ist konfiguriert
- Ingress Controller ist vorhanden, z. B. NGINX Ingress
- Optional bei lokalem Cluster: Host-Eintrag für `backstage.local`

## Deployment

```bash
kubectl apply -k overlays/dev
```

## Status prüfen

```bash
kubectl get pods -n backstage
kubectl get svc -n backstage
kubectl get ingress -n backstage
```

## Logs prüfen

```bash
kubectl logs -n backstage deployment/backstage
```

## Zugriff

Bei lokalem Cluster muss `backstage.local` auf die Cluster-IP oder Ingress-IP zeigen.

Beispiel mit Minikube:

```bash
minikube ip
```

Danach `/etc/hosts` ergänzen:

```text
<MINIKUBE-IP> backstage.local
```

Aufruf im Browser:

```text
http://backstage.local
```

## Acceptance Criteria Nachweis

| Acceptance Criteria | Nachweis |
|---|---|
| Backstage is deployed within Kubernetes | `kubectl get deployment -n backstage` |
| All required pods are in the `Running` state | `kubectl get pods -n backstage` |
| The Backstage web interface is reachable | Browser-Test mit `http://backstage.local` |
| Configuration is stored in version control | Kustomize-Manifeste im Repository |
| Deployment steps are documented | Dieses Dokument |
