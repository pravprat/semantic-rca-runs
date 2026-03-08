# Semantic RCA Report

## Incident Window

2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:29:58.127428+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Child Incidents: I2
Classification: Primary incident

---

## Primary Trigger

Timestamp: 2023-01-27T18:28:43.254658Z
Actor: system:node:k8s-node-1-perfspec
Action: list configmaps
Response: HTTP 403

---

## Root Cause Candidate

Component: **system:node:k8s-node-1-perfspec**

### Cluster Behavior

system:node:k8s-node-1-perfspec operation resource → HTTP 403 (authorization/client errors)

Detected **5 anomalous events** (trigger_score=2.501197).

Confidence: **medium** (0.593)

---

## Representative Failure

Timestamp: 2023-01-27T18:28:43.254658Z
Actor: system:node:k8s-node-1-perfspec
Action: list configmaps
Response: HTTP 403

---

## Error Distribution

4xx: 5
2xx: 1

---

## Propagation Chain

gatekeeper-system/gatekeeper-admin → system:apiserver → system:node:k8s-node-1-perfspec → system:kube-controller-manager → kubernetes-admin

---

## Propagation Delays

gatekeeper-system/gatekeeper-admin → system:apiserver : 34s
system:apiserver → system:node:k8s-node-1-perfspec : 1s
system:node:k8s-node-1-perfspec → system:kube-controller-manager : 0s
system:kube-controller-manager → kubernetes-admin : 10s

---

## Failure Timeline

2023-01-27T18:28:08.160137Z — gatekeeper-system/gatekeeper-admin (HTTP 503)
2023-01-27T18:28:42.247463Z — system:apiserver (HTTP 404)
2023-01-27T18:28:43.254658Z — system:node:k8s-node-1-perfspec (HTTP 403)
2023-01-27T18:28:43.778767Z — system:kube-controller-manager (HTTP 200)
2023-01-27T18:28:54.549269Z — kubernetes-admin (HTTP 404)

---

## Confidence Reasoning

- cluster exhibits highest trigger anomaly score
- cluster contains largest burst of error responses
- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **system:node:k8s-node-1-perfspec**, described as: **system:node:k8s-node-1-perfspec operation resource → HTTP 403 (authorization/client errors)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
