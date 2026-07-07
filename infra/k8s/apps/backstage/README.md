# Backstage PoC Deployment mit Kustomize

Dieses Verzeichnis enthält ein minimales Kubernetes-Deployment für Backstage als Proof of Concept.

## Struktur

```text
backstage-poc-kustomize/
├── base/
│   ├── namespace.yaml
│   ├── configmap.yaml
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── ingress.yaml
│   └── kustomization.yaml
├── overlays/
│   └── dev/
│       ├── kustomization.yaml
│       ├── patch-config-url.yaml
│       ├── patch-ingress-host.yaml
│       └── patch-resources.yaml
└── docs/
    └── deployment-steps.md
```

## Deployment

```bash
kubectl apply -k overlays/dev
```

## Prüfen

```bash
kubectl get all -n backstage
kubectl get ingress -n backstage
kubectl logs -n backstage deployment/backstage
```

## Wichtige Anpassungen

Für den PoC ist nur der Host wichtig:

- `base/ingress.yaml`
- `overlays/dev/patch-ingress-host.yaml`
- `base/configmap.yaml`
- `overlays/dev/patch-config-url.yaml`

Standardwert:

```text
backstage.local
```

## Hinweis

Es wird bewusst das fertige Image `ghcr.io/backstage/backstage:latest` verwendet. Für den PoC reicht das aus, um das Kubernetes-Deployment und die Erreichbarkeit der Weboberfläche zu validieren. Ein eigenes Image ist erst notwendig, wenn eigene Plugins, Authentifizierung oder produktionsnahe Anpassungen umgesetzt werden.
