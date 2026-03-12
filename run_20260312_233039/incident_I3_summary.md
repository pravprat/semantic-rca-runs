# Semantic RCA Report

## Incident Window

2026-02-18T00:00:00.029922+00:00 → 2026-02-18T00:12:52.091208+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-18T00:00:00.029922139Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Root Cause Candidate

Component: **vault**

### Cluster Behavior

vault operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.321)

---

## Representative Failure

Timestamp: 2026-02-18T00:12:31.75070989Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Error Distribution

unknown: 42

---

## Propagation Chain

vault

---

## Propagation Delays

Unable to compute propagation delay

---

## Failure Timeline

2026-02-18T00:00:00.029922139Z — vault (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **vault**, described as: **vault operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
