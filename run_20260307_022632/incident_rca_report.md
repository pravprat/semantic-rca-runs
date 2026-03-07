# Semantic RCA Report

---
# Incident I1

## Incident Window
2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:29:58.127428+00:00

## Root Cause

Cluster: `C163`
Score: 92.67

### Cluster Behavior
unknown actor   → None (unknown outcome)

### Trigger Explanation
system:serviceaccount:gatekeeper-system:gatekeeper-admin attempted to list assignmetadata via  resulting in HTTP 404

### Key Signals
- trigger_score: 2.912427
- error_count: 108
- graph_out_weight: 10.95
- graph_in_weight: 5.0

### Blast Radius
Affected downstream clusters: **5**

### Causal Propagation
```mermaid
flowchart TD
C163 --> C152["unknown actor   → None (unknown outcome)"]
C163 --> C119["unknown actor   → None (unknown outcome)"]
C163 --> C200["unknown actor   → None (unknown outcome)"]
C163 --> C21["unknown actor   → None (unknown outcome)"]
C163 --> C78["unknown actor   → None (unknown outcome)"]
```

### Primary Evidence Event
```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,
```

## Other Possible Contributors

| Rank | Cluster | Behavior | Score | Errors |
|------|--------|----------|------|------|
| 2 | C165 | unknown actor   → None (unknown outcome) | 33.87 | 28 |
| 3 | C131 | unknown actor   → None (unknown outcome) | 25.76 | 16 |
| 4 | C81 | unknown actor   → None (unknown outcome) | 25.69 | 10 |
| 5 | C19 | unknown actor   → None (unknown outcome) | 25.01 | 114 |

---
# Incident I2

## Incident Window
2023-01-27T18:30:58.127428+00:00 → 2023-01-27T18:31:48.127428+00:00

## Root Cause

Cluster: `C163`
Score: 82.89

### Cluster Behavior
unknown actor   → None (unknown outcome)

### Trigger Explanation
system:serviceaccount:gatekeeper-system:gatekeeper-admin attempted to list assignmetadata via  resulting in HTTP 404

### Key Signals
- trigger_score: 2.912427
- error_count: 108
- graph_out_weight: 7.150000000000001
- graph_in_weight: 0.0

### Blast Radius
Affected downstream clusters: **5**

### Causal Propagation
```mermaid
flowchart TD
C163 --> C152["unknown actor   → None (unknown outcome)"]
C163 --> C119["unknown actor   → None (unknown outcome)"]
C163 --> C200["unknown actor   → None (unknown outcome)"]
C163 --> C21["unknown actor   → None (unknown outcome)"]
C163 --> C104["unknown actor   → None (unknown outcome)"]
```

### Primary Evidence Event
```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,
```

## Other Possible Contributors

| Rank | Cluster | Behavior | Score | Errors |
|------|--------|----------|------|------|
| 2 | C15 | unknown actor   → None (unknown outcome) | 81.77 | 23 |
| 3 | C0 | unknown actor   → None (unknown outcome) | 47.13 | 90 |
| 4 | C77 | unknown actor   → None (unknown outcome) | 32.46 | 36 |
| 5 | C117 | unknown actor   → None (unknown outcome) | 31.19 | 4 |
