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

Timestamp: 2023-01-27T18:28:42.240231Z
Actor: system:serviceaccount:kube-system:replicaset-controller
Action: create pods
Response: HTTP 403

---

## Root Cause Candidate

Component: **kube-system/replicaset-controller**

### Cluster Behavior

unknown actor   → None (unknown outcome)

Detected **16 anomalous events** (trigger_score=1.526411).

Confidence: **medium** (0.577)

---

## Representative Failure

Timestamp: 2023-01-27T18:28:42.240231Z
Actor: system:serviceaccount:kube-system:replicaset-controller
Action: create pods
Response: HTTP 403

---

## Error Distribution

4xx: 16
2xx: 5

---

## Propagation Chain

gatekeeper-system/gatekeeper-admin → kube-system/replicaset-controller → system:apiserver → system:kube-controller-manager → kubernetes-admin

---

## Propagation Delays

gatekeeper-system/gatekeeper-admin → kube-system/replicaset-controller : 34s
kube-system/replicaset-controller → system:apiserver : 0s
system:apiserver → system:kube-controller-manager : 1s
system:kube-controller-manager → kubernetes-admin : 10s

---

## Failure Timeline

2023-01-27T18:28:08.160137Z — gatekeeper-system/gatekeeper-admin (HTTP 503)
2023-01-27T18:28:42.240231Z — kube-system/replicaset-controller (HTTP 403)
2023-01-27T18:28:42.247463Z — system:apiserver (HTTP 404)
2023-01-27T18:28:43.778767Z — system:kube-controller-manager (HTTP 200)
2023-01-27T18:28:54.549269Z — kubernetes-admin (HTTP 404)

---

## Confidence Reasoning

- cluster exhibits highest trigger anomaly score
- cluster contains largest burst of error responses
- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **kube-system/replicaset-controller**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
