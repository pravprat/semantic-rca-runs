# Semantic RCA Report

## Incident Window

2026-02-17T23:59:41.845137+00:00 → 2026-02-18T00:10:14.093645+00:00

Incident Severity: **Low**
Incident Type: **Operational anomaly**

---

## Incident Relationships

Classification: Primary incident

---

## Primary Trigger

Timestamp: 2026-02-17T23:59:47.096923363Z
Actor:  Servers: [{ Addr: mongodb-sharded:27017
Action:  Type: Unknown  Last error: dial tcp 10.43.252.183:27017: connect: connection refused }
Response: HTTP unknown

---

## Root Cause Candidate

Component: **utility**

### Cluster Behavior

utility operation resource (unknown outcome)

Detected **0 anomalous events** (trigger_score=0.0).

Confidence: **low** (0.309)

---

## Representative Failure

Timestamp: 2026-02-18T00:10:14.093645317Z
Actor:  Servers: [{ Addr: mongodb-sharded:27017
Action:  Type: Unknown  Last error: dial tcp 10.43.252.183:27017: connect: connection refused }
Response: HTTP unknown

---

## Error Distribution

unknown: 8

---

## Propagation Chain

utility

---

## Propagation Delays

utility → utility : 0s
utility → utility : 0s
utility → utility : 0s
utility → utility : 5s

---

## Failure Timeline

2026-02-17T23:59:41.845322Z — utility (HTTP None)
2026-02-17T23:59:41.845334Z — utility (HTTP None)
2026-02-17T23:59:41.845446Z — utility (HTTP None)
2026-02-17T23:59:42.096246Z — utility (HTTP None)
2026-02-17T23:59:47.096923363Z — utility (HTTP None)

---

## Confidence Reasoning

- events occur earliest in incident timeline

---

## Deterministic Conclusion

The earliest anomaly burst originates from **utility**, described as: **utility operation resource (unknown outcome)**. Temporal ordering, error concentration, and trigger score identify this component as the most probable origin of the incident.
