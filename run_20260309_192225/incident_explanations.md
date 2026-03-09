# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163
Behavior: Gatekeeper policy evaluation failures
Score: 55.86

- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 5

### Cluster C19
Behavior: kubernetes-admin get configmaps client failures (HTTP 404)
Score: 28.77

- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 128 events
- Error burst detected: 114 anomalous events
- Trigger proximity to incident start: 0.578
- Downstream clusters affected: 5

### Cluster C165
Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)
Score: 28.43

- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 34 events
- Error burst detected: 28 anomalous events
- Trigger proximity to incident start: 0.028

### Cluster C111
Behavior: Node RBAC permission failures
Score: 21.05

- Behavior: system:node:k8s-node-1-perfspec list configmaps (HTTP 403)
- Cluster size: 6 events
- Error burst detected: 5 anomalous events
- Trigger proximity to incident start: 0.681

### Cluster C131
Behavior: Service account lookup failures
Score: 20.78

- Behavior: system:apiserver get serviceaccounts (HTTP 404)
- Cluster size: 16 events
- Error burst detected: 16 anomalous events
- Trigger proximity to incident start: 0.69

---
# Incident I2

### Cluster C0
Behavior: kubernetes-admin get configmaps client failures (HTTP 404)
Score: 44.46

- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 90 events
- Error burst detected: 90 anomalous events
- Trigger proximity to incident start: 0.955

### Cluster C117
Behavior: k8s-node-1-perfspec patch events client failures (HTTP 404)
Score: 28.79

- Behavior: system:node:k8s-node-1-perfspec patch events (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.616

### Cluster C15
Behavior: argocd-applicationset-controller get secrets operations (HTTP 200)
Score: 27.18

- Behavior: system:serviceaccount:argo-cd:argocd-applicationset-controller get secrets (HTTP 200)
- Cluster size: 99 events
- Error burst detected: 23 anomalous events
- Trigger proximity to incident start: 0.951
- Downstream clusters affected: 5

### Cluster C182
Behavior: Secret lookup failures
Score: 27.11

- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733
- Downstream clusters affected: 5

### Cluster C188
Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)
Score: 27.08

- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.331
