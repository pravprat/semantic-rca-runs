# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163
Behavior: Gatekeeper policy evaluation failures
Score: 52.26

- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 5

### Cluster C165
Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)
Score: 28.43

- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 34 events
- Error burst detected: 28 anomalous events
- Trigger proximity to incident start: 0.028

### Cluster C220
Behavior: replicaset-controller create pods client failures (HTTP 403)
Score: 26.04

- Behavior: system:serviceaccount:kube-system:replicaset-controller create pods (HTTP 403)
- Cluster size: 21 events
- Error burst detected: 16 anomalous events
- Trigger proximity to incident start: 0.69
- Downstream clusters affected: 5

### Cluster C19
Behavior: kubernetes-admin get configmaps client failures (HTTP 404)
Score: 25.11

- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 128 events
- Error burst detected: 114 anomalous events
- Trigger proximity to incident start: 0.578

### Cluster C67
Behavior: kubernetes-admin create services operations (HTTP 201)
Score: 23.88

- Behavior: kubernetes-admin create services (HTTP 201)
- Cluster size: 46 events
- Error burst detected: 9 anomalous events
- Trigger proximity to incident start: 0.575
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
Score: 33.78

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

### Cluster C182
Behavior: Secret lookup failures
Score: 21.97

- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733

### Cluster C163
Behavior: Gatekeeper policy evaluation failures
Score: 20.43

- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 5
