# Semantic RCA Report

## Incident Window

2026-02-17T23:59:16.447354+00:00 → 2026-02-18T00:11:42.798579+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-17T23:59:16.703964Z
Actor:  etc.)
Action: unknown unknown
Response: HTTP unknown

---

## Root Cause Candidate

Component: **vector-store-chart**

### Cluster Behavior

vector-store-chart operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.307)

---

## Representative Failure

Timestamp: 2026-02-17T23:59:16.703964Z
Actor:  etc.)
Action: unknown unknown
Response: HTTP unknown

---

## Error Distribution

unknown: 7

---

## Propagation Chain

vector-store-chart

---

## Propagation Delays

vector-store-chart → vector-store-chart : 0s
vector-store-chart → vector-store-chart : 0s
vector-store-chart → vector-store-chart : 0s
vector-store-chart → vector-store-chart : 0s

---

## Failure Timeline

2026-02-17T23:59:16.453389Z — vector-store-chart (HTTP None)
2026-02-17T23:59:16.453411Z — vector-store-chart (HTTP None)
2026-02-17T23:59:16.453488Z — vector-store-chart (HTTP None)
2026-02-17T23:59:16.703904Z — vector-store-chart (HTTP None)
2026-02-17T23:59:16.703964Z — vector-store-chart (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **vector-store-chart**, described as: **vector-store-chart operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
