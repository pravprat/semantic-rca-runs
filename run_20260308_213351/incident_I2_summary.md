# Semantic RCA Report

## Incident Window

2023-01-27T18:30:58.127428+00:00 → 2023-01-27T18:31:48.127428+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2023-01-27T18:31:06.473918Z
Actor: system:kube-controller-manager
Action: get serviceaccounts
Response: HTTP 200

---

## Root Cause Candidate

Component: **kube-system/deployment-controller**

### Cluster Behavior

kube-system/deployment-controller operation resource → HTTP 200 (successful operations)

Detected **11 anomalous events** (trigger_score=0.136381).

Confidence: **medium** (0.702)

---

## Representative Failure

Timestamp: 2023-01-27T18:31:07.437877Z
Actor: system:serviceaccount:kube-system:deployment-controller
Action: update deployments
Response: HTTP 200

---

## Error Distribution

2xx: 74
4xx: 11

---

## Propagation Chain

gatekeeper-system/gatekeeper-admin → kubernetes-admin → system:kube-controller-manager → system:node:k8s-node-1-perfspec

---

## Propagation Delays

gatekeeper-system/gatekeeper-admin → kubernetes-admin : 177s
kubernetes-admin → system:kube-controller-manager : 0s
system:kube-controller-manager → system:node:k8s-node-1-perfspec : 19s
system:node:k8s-node-1-perfspec → kubernetes-admin : 17s

---

## Failure Timeline

2023-01-27T18:28:08.160137Z — gatekeeper-system/gatekeeper-admin (HTTP 503)
2023-01-27T18:31:05.897828Z — kubernetes-admin (HTTP 404)
2023-01-27T18:31:06.473918Z — system:kube-controller-manager (HTTP 200)
2023-01-27T18:31:26.258728Z — system:node:k8s-node-1-perfspec (HTTP 404)
2023-01-27T18:31:43.335010Z — kubernetes-admin (HTTP 404)

---

## Confidence Reasoning

- cluster exhibits highest trigger anomaly score
- cluster contains largest burst of error responses
- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **kube-system/deployment-controller**, described as: **kube-system/deployment-controller operation resource → HTTP 200 (successful operations)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
