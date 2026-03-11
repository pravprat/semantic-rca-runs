# Semantic RCA Report

---
# Incident I1

## Incident Window
2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:29:58.127428+00:00

## Root Cause

Cluster: `C163`
Score: 87.14


Component: gatekeeper-admin
Failure Mode: resource_lookup_failure
Status Class: 4xx

Behavior:
Gatekeeper policy evaluation failures

### Cluster Behavior
system:serviceaccount:gatekeeper-system:gatekeeper-admin list assignmetadata → HTTP 404 (authorization/client errors)

### Trigger Explanation
system:serviceaccount:gatekeeper-system:gatekeeper-admin attempted to list assignmetadata via  resulting in HTTP 404

### Key Signals
- trigger_score: 2.912427
- error_count: 108
- graph_out_weight: 10.95
- graph_in_weight: 5.0

### Blast Radius
Affected downstream clusters: **11**

### Trigger / Lag / Lead

- Trigger: system:serviceaccount:gatekeeper-system:gatekeeper-admin list assignmetadata → HTTP 404 (authorization/client errors)
- Lag: unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster
- Lead: unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster

### Causal Propagation
```mermaid
flowchart TD
C163["C163"] --> C157["C157"]
C163["C163"] --> C168["C168"]
C163["C163"] --> C200["C200"]
C163["C163"] --> C205["C205"]
C163["C163"] --> C21["C21"]
C163["C163"] --> C39["C39"]
C163["C163"] --> C57["C57"]
C163["C163"] --> C67["C67"]
C163["C163"] --> C75["C75"]
C163["C163"] --> C9["C9"]
C163["C163"] --> C96["C96"]
```

### Primary Evidence Event
```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,
```

## Other Possible Contributors

| Rank | Cluster | Behavior | Score | Errors |
|------|--------|----------|------|------|
| 2 | C67 | kubernetes-admin create deployments in namespace my-argo-cd-argocd-applicationset-controller → HTTP 201 (successful operations) | 46.04 | 9 |
| 3 | C165 | kubernetes-admin delete rolebindings in namespace my-cert-manager-startupapicheck:create-cert → HTTP 200 (successful operations) | 36.12 | 28 |
| 4 | C19 | kubernetes-admin get daemonsets in namespace my-prometheus-prometheus-node-exporter → HTTP 404 (authorization/client errors) | 32.13 | 114 |
| 5 | C112 | kubernetes-admin delete rolebindings in namespace my-ingress-nginx-admission → HTTP 404 (authorization/client errors) | 32.05 | 12 |

---
# Incident I2

## Incident Window
2023-01-27T18:30:58.127428+00:00 → 2023-01-27T18:31:48.127428+00:00

## Root Cause

Cluster: `C0`
Score: 90.25


Component: argocd
Failure Mode: resource_lookup_failure
Status Class: 4xx

Behavior:
kubernetes-admin get configmaps client failures (HTTP 404)

### Cluster Behavior
kubernetes-admin get rolebindings in namespace my-argo-cd-argocd-applicationset-controller → HTTP 404 (authorization/client errors)

### Trigger Explanation
kubernetes-admin attempted to get rolebindings via  resulting in HTTP 404

### Key Signals
- trigger_score: 4.721854
- error_count: 90
- graph_out_weight: 10.95
- graph_in_weight: 0.0

### Blast Radius
Affected downstream clusters: **10**

### Trigger / Lag / Lead

- Trigger: kubernetes-admin get rolebindings in namespace my-argo-cd-argocd-applicationset-controller → HTTP 404 (authorization/client errors)
- Lag: unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster
- Lead: unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster ; unknown cluster

### Causal Propagation
```mermaid
flowchart TD
C0["C0"] --> C114["C114"]
C0["C0"] --> C125["C125"]
C0["C0"] --> C137["C137"]
C0["C0"] --> C168["C168"]
C0["C0"] --> C191["C191"]
C0["C0"] --> C200["C200"]
C0["C0"] --> C29["C29"]
C0["C0"] --> C57["C57"]
C0["C0"] --> C67["C67"]
C0["C0"] --> C87["C87"]
```

### Primary Evidence Event
```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:06.032926Z,kubernetes-admin,get,rolebindings,,my-argo-cd-argocd-applicationset-controller,,/apis/rbac.authorization.k8s.io/v1/namespaces/argo-cd/rolebindings/my-argo-cd-argocd-applicationset-controller,ffb58937-bfd6-4945-b8d0-ce40f76d14ba,ResponseComplete,404,,,
```

## Other Possible Contributors

| Rank | Cluster | Behavior | Score | Errors |
|------|--------|----------|------|------|
| 2 | C117 | system:node:k8s-node-1-perfspec patch events in namespace my-loki-logs-8mj42.173e3c8107533d12 → HTTP 404 (authorization/client errors) | 38.54 | 4 |
| 3 | C163 | system:serviceaccount:gatekeeper-system:gatekeeper-admin list assignmetadata → HTTP 404 (authorization/client errors) | 38.46 | 108 |
| 4 | C188 | kubernetes-admin get rolebindings in namespace my-kubernetes-dashboard → HTTP 404 (authorization/client errors) | 34.49 | 4 |
| 5 | C182 | kubernetes-admin create secrets in namespace my-redis → HTTP 201 (successful operations) | 30.36 | 13 |
