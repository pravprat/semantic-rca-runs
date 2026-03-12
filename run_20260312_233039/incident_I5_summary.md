# Semantic RCA Report

## Incident Window

2026-02-18T00:00:06.996853+00:00 → 2026-02-18T00:12:45.940965+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-18T00:00:06.996853924Z
Actor:  Servers: [{ Addr: localhost:27017
Action:  Type: Unknown  Last error: dial tcp [::1]:27017: connect: connection refused }
Response: HTTP unknown

---

## Root Cause Candidate

Component: **metrics**

### Cluster Behavior

metrics operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.321)

---

## Representative Failure

Timestamp: 2026-02-18T00:06:36.99694626Z
Actor:  Servers: [{ Addr: localhost:27017
Action:  Type: Unknown  Last error: dial tcp [::1]:27017: connect: connection refused }
Response: HTTP unknown

---

## Error Distribution

unknown: 100

---

## Propagation Chain

metrics

---

## Propagation Delays

Unable to compute propagation delay

---

## Failure Timeline

2026-02-18T00:00:06.996853924Z — metrics (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **metrics**, described as: **metrics operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
