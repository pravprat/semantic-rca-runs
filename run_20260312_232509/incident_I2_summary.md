# Semantic RCA Report

## Incident Window

2026-02-18T00:00:00.227247+00:00 → 2026-02-18T00:12:52.289768+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-18T00:00:00.227247211Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Root Cause Candidate

Component: **proxy**

### Cluster Behavior

proxy operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.311)

---

## Representative Failure

Timestamp: 2026-02-18T00:10:36.365249265Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Error Distribution

unknown: 61

---

## Propagation Chain

proxy

---

## Propagation Delays

proxy → proxy : 31s
proxy → proxy : 0s
proxy → proxy : 44s
proxy → proxy : 0s

---

## Failure Timeline

2026-02-18T00:00:00.227247211Z — proxy (HTTP None)
2026-02-18T00:00:31.672663012Z — proxy (HTTP None)
2026-02-18T00:00:31.672665639Z — proxy (HTTP None)
2026-02-18T00:01:15.922447899Z — proxy (HTTP None)
2026-02-18T00:01:15.922651223Z — proxy (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **proxy**, described as: **proxy operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
