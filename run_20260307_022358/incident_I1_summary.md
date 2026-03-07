# Semantic RCA Report

## Incident Window

2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:29:58.127428+00:00

Incident Severity: **Medium**
Incident Type: **Control-plane service failure**

---

## Incident Relationships

Child Incidents: I2
Classification: Primary incident

---

## Primary Trigger

Timestamp: 2023-01-27T18:28:08.160137Z
Actor: system:serviceaccount:gatekeeper-system:gatekeeper-admin
Action: list constrainttemplatepodstatuses
Response: HTTP 503

---

## Root Cause Candidate

Component: **gatekeeper-system/gatekeeper-admin**

### Cluster Behavior

unknown actor   → None (unknown outcome)

Detected **108 anomalous events** (trigger_score=2.912427).

Confidence: **high** (0.907)

---

## Representative Failure

Timestamp: 2023-01-27T18:28:22.470778Z
Actor: system:serviceaccount:gatekeeper-system:gatekeeper-admin
Action: list assignmetadata
Response: HTTP 404

---

## Error Distribution

2xx: 4
5xx: 1
4xx: 95

---

## Propagation Chain

system:node:k8s-node-1-perfspec → gatekeeper-system/gatekeeper-admin → system:apiserver → kubernetes-admin

---

## Propagation Delays

system:node:k8s-node-1-perfspec → gatekeeper-system/gatekeeper-admin : 0s
gatekeeper-system/gatekeeper-admin → system:apiserver : 34s
system:apiserver → kubernetes-admin : 12s
kubernetes-admin → kubernetes-admin : 60s

---

## Failure Timeline

2023-01-27T18:28:08.131819Z — system:node:k8s-node-1-perfspec (HTTP 403)
2023-01-27T18:28:08.160137Z — gatekeeper-system/gatekeeper-admin (HTTP 503)
2023-01-27T18:28:42.247463Z — system:apiserver (HTTP 404)
2023-01-27T18:28:54.549269Z — kubernetes-admin (HTTP 404)
2023-01-27T18:29:55.101864Z — kubernetes-admin (HTTP 404)

---

## Confidence Reasoning

- cluster exhibits highest trigger anomaly score
- cluster contains largest burst of error responses
- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **gatekeeper-system/gatekeeper-admin**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
