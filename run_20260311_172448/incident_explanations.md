# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C16

Behavior: kube-apiserver server failures (HTTP 502)

Score: 45.11

Root Cause: milvus service_failure

Trigger Event: W1024 23:56:04.473710       1 reflector.go:569] storage/cacher.go:/milvus.io/milvuses: failed to list milvus.io/v1alpha1, Kind=Milvus: conversion webhook for milvus.io/v1beta1, Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443, code 502: 502 Bad Gateway


Blast Radius: 0


- Behavior: kube-apiserver   (HTTP 502)
- Cluster size: 19 events
- Error burst detected: 19 anomalous events
- Trigger proximity to incident start: 0.977

### Cluster C6

Behavior: kube-apiserver server failures (HTTP 502)

Score: 28.48

Root Cause: milvus service_failure

Trigger Event: E1024 23:56:04.473736       1 cacher.go:478] cacher (milvuses.milvus.io): unexpected ListAndWatch error: failed to list milvus.io/v1alpha1, Kind=Milvus: conversion webhook for milvus.io/v1beta1, Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443, code 502: 502 Bad Gateway; reinitializing...


Blast Radius: 0


- Behavior: kube-apiserver   (HTTP 502)
- Cluster size: 1190 events
- Error burst detected: 1190 anomalous events
- Trigger proximity to incident start: 1.0

### Cluster C15

Behavior: kube-apiserver server failures (HTTP 502)

Score: 27.67

Root Cause: milvus service_failure

Trigger Event: W1024 23:56:56.296325       1 reflector.go:569] storage/cacher.go:/milvus.io/milvuses: failed to list milvus.io/v1alpha1, Kind=Milvus: conversion webhook for milvus.io/v1beta1, Kind=Milvus failed: Post "https://aide-system-milvus-operator-webhook-service.aide-system.svc:443/convert?timeout=30s": proxy error from 127.0.0.1:9345 while dialing 10.42.193.206:9443, code 502: 502 Bad Gateway


Blast Radius: 0


- Behavior: kube-apiserver   (HTTP 502)
- Cluster size: 1162 events
- Error burst detected: 1162 anomalous events
- Trigger proximity to incident start: 1.0
