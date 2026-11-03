# K8s Ingress

Kubernetes Ingress resource for the RoboShop frontend service. Routes external traffic to the frontend service via an ALB.

## Files

| File | Purpose |
|---|---|
| `ingress.yaml` | Ingress resource with ALB annotations + TLS |

## Key Patterns

- **ALB Ingress** — AWS Load Balancer Controller annotations
- **TLS termination** — ACM certificate for HTTPS
- **Path-based routing** — `/` → frontend service

## Quick Start

```bash
kubectl apply -f ingress.yaml
```

## Related Practice
