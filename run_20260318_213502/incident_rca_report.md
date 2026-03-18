# Semantic RCA Report

---
## Incident I1

Window: 2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:29:18.127428+00:00

Primary Issue: **Authorization / RBAC failure**

Repeated 401/403 failures across one or more system actors indicate an authorization or RBAC issue.

- Score: 0.99
- Confidence: high (0.99)
- Service: system:serviceaccount:kube-system:replicaset-controller
- Operation: create pods
- Status Class: 4xx

---
## Incident I2

Window: 2023-01-27T18:30:38.127428+00:00 → 2023-01-27T18:30:48.127428+00:00

Primary Issue: **Dominant failure pattern**

Most concentrated failure pattern is get unknown with status class 2xx.

- Score: 0.5
- Confidence: low (0.5)
- Service: system:serviceaccount:cert-manager:my-cert-manager-startupapicheck
- Operation: get unknown
- Status Class: 2xx
