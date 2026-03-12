# Semantic RCA Report

## Incident Window

2026-02-17T23:59:40.512419+00:00 → 2026-02-18T00:10:03.763798+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-17T23:59:45.765046768Z
Actor:  Servers: [{ Addr: mongodb-sharded:27017
Action:  Type: Unknown  Last error: dial tcp 10.43.252.183:27017: connect: connection refused }
Response: HTTP unknown

---

## Root Cause Candidate

Component: **policy-engine-chart**

### Cluster Behavior

policy-engine-chart operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.315)

---

## Representative Failure

Timestamp: 2026-02-18T00:04:52.77920242Z
Actor:  Servers: [{ Addr: mongodb-sharded:27017
Action:  Type: Unknown  Last error: dial tcp 10.43.252.183:27017: connect: connection refused }
Response: HTTP unknown

---

## Error Distribution

unknown: 7

---

## Propagation Chain

policy-engine-chart

---

## Propagation Delays

policy-engine-chart → policy-engine-chart : 0s
policy-engine-chart → policy-engine-chart : 0s
policy-engine-chart → policy-engine-chart : 0s
policy-engine-chart → policy-engine-chart : 5s

---

## Failure Timeline

2026-02-17T23:59:40.512419Z — policy-engine-chart (HTTP None)
2026-02-17T23:59:40.512753Z — policy-engine-chart (HTTP None)
2026-02-17T23:59:40.763873Z — policy-engine-chart (HTTP None)
2026-02-17T23:59:40.764184Z — policy-engine-chart (HTTP None)
2026-02-17T23:59:45.765046768Z — policy-engine-chart (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **policy-engine-chart**, described as: **policy-engine-chart operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
