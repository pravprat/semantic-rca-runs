# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163
Behavior: Gatekeeper policy evaluation failures
Score: 54.66

- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 5

### Cluster C19
Behavior: kubernetes-admin get configmaps client failures (HTTP 404)
Score: 32.77

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
Score: 26.15

- Behavior: system:node:k8s-node-1-perfspec list configmaps (HTTP 403)
- Cluster size: 6 events
- Error burst detected: 5 anomalous events
- Trigger proximity to incident start: 0.681
- Downstream clusters affected: 5

### Cluster C31
Behavior: my-kube-prometheus-stack-operator get secrets operations (HTTP 200)
Score: 24.19

- Behavior: system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator get secrets (HTTP 200)
- Cluster size: 1343 events
- Error burst detected: 222 anomalous events
- Trigger proximity to incident start: 0.482
- Downstream clusters affected: 5

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
Score: 34.58

- Behavior: system:node:k8s-node-1-perfspec patch events (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.616
- Downstream clusters affected: 5

### Cluster C188
Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)
Score: 27.08

- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.331

### Cluster C27
Behavior: deployment-controller update deployments operations (HTTP 200)
Score: 25.83

- Behavior: system:serviceaccount:kube-system:deployment-controller update deployments (HTTP 200)
- Cluster size: 85 events
- Error burst detected: 11 anomalous events
- Trigger proximity to incident start: 0.945
- Downstream clusters affected: 5

### Cluster C182
Behavior: Secret lookup failures
Score: 21.97

- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733
