# Semantic RCA Report

## Incident Window

2026-02-18T00:00:46.039785+00:00 → 2026-02-18T00:11:14.199804+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-18T00:00:46.290357Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Root Cause Candidate

Component: **metadata-chart**

### Cluster Behavior

metadata-chart operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.307)

---

## Representative Failure

Timestamp: 2026-02-18T00:00:46.290357Z
Actor: unknown
Action: unknown unknown
Response: HTTP unknown

---

## Error Distribution

unknown: 7

---

## Propagation Chain

metadata-chart

---

## Propagation Delays

metadata-chart → metadata-chart : 0s
metadata-chart → metadata-chart : 0s
metadata-chart → metadata-chart : 0s
metadata-chart → metadata-chart : 5s

---

## Failure Timeline

2026-02-18T00:00:46.039785Z — metadata-chart (HTTP None)
2026-02-18T00:00:46.039838Z — metadata-chart (HTTP None)
2026-02-18T00:00:46.040055Z — metadata-chart (HTTP None)
2026-02-18T00:00:46.290357Z — metadata-chart (HTTP None)
2026-02-18T00:00:51.291103582Z — metadata-chart (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **metadata-chart**, described as: **metadata-chart operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
