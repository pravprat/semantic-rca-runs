# Semantic RCA Report

---
# Incident I1

## Incident Window
2025-10-24T23:50:00.933281+00:00 → 2025-10-24T23:50:10.933281+00:00

## Root Cause

Cluster: `C16`
Score: 45.11


Component: milvus
Failure Mode: service_failure
Status Class: 5xx

Behavior:
kube-apiserver server failures (HTTP 502)

### Cluster Behavior
Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443 code 502: 502 Bad Gateway resource (unknown outcome)

### Trigger Explanation
 Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443 attempted to  code 502: 502 Bad Gateway  via  resulting in HTTP 

### Key Signals
- trigger_score: 3.000939
- error_count: 19
- graph_out_weight: 0.0
- graph_in_weight: 0.0

### Blast Radius
Affected downstream clusters: **0**

### Trigger / Lag / Lead

- Trigger: Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443 code 502: 502 Bad Gateway resource (unknown outcome)
- Lag: none detected
- Lead: none detected

### Causal Propagation
No downstream propagation detected.

### Primary Evidence Event
```
W1024 23:56:04.473710       1 reflector.go:569] storage/cacher.go:/milvus.io/milvuses: failed to list milvus.io/v1alpha1, Kind=Milvus: conversion webhook for milvus.io/v1beta1, Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443, code 502: 502 Bad Gateway
```

## Other Possible Contributors

| Rank | Cluster | Behavior | Score | Errors |
|------|--------|----------|------|------|
| 2 | C6 | Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443 code 502: 502 Bad Gateway; reinitializing... resource (unknown outcome) | 28.48 | 1190 |
| 3 | C15 | Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443 code 502: 502 Bad Gateway resource (unknown outcome) | 27.67 | 1162 |
