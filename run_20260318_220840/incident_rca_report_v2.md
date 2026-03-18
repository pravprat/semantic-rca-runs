# Semantic RCA Report

---
## Incident I1

Window: 2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:29:18.127428+00:00

Root Cause: **Authorization / RBAC failure**

Repeated authorization failures were detected. The earliest pattern is watch configmaps with 4xx. The failure affects 5 actor(s), including 7 control-plane pattern(s).

- Confidence: high (0.99)

---
## Incident I2

Window: 2023-01-27T18:30:38.127428+00:00 → 2023-01-27T18:30:48.127428+00:00

Root Cause: **Dominant failure domain**

A dominant failure domain was identified from the incident patterns. The earliest pattern is get nodes with status class 2xx.

- Confidence: high (0.84)
