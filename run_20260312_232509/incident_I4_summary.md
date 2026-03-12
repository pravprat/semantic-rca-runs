# Semantic RCA Report

## Incident Window

2026-02-18T00:00:00.235139+00:00 → 2026-02-18T00:12:59.734973+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-18T00:00:50.296057301Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Root Cause Candidate

Component: **etcd**

### Cluster Behavior

etcd operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.288)

---

## Representative Failure

Timestamp: 2026-02-18T00:00:50.296057301Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Error Distribution

unknown: 5

---

## Propagation Chain

etcd

---

## Propagation Delays

etcd → etcd : 0s
etcd → etcd : 1s
etcd → etcd : 0s
etcd → etcd : 47s

---

## Failure Timeline

2026-02-18T00:00:00.258007902Z — etcd (HTTP None)
2026-02-18T00:00:00.258081718Z — etcd (HTTP None)
2026-02-18T00:00:02.088927262Z — etcd (HTTP None)
2026-02-18T00:00:02.73498476Z — etcd (HTTP None)
2026-02-18T00:00:50.296057301Z — etcd (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **etcd**, described as: **etcd operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
