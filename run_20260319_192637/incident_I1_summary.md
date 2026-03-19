# Incident I1

## Incident Window

2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:58:08.127428+00:00

## Root Cause

**Control-plane / service failure**

Repeated 5xx failures indicate an unstable or failing service. The earliest service-failure pattern is get unknown from system:serviceaccount:cert-manager:my-cert-manager-cainjector.

## Why this is the Root Cause

- Earliest observed failure pattern in the incident window
- Affects multiple system actors (systemic impact)
- Impacts control-plane components
- Indicates service instability (5xx errors)
- High trigger intensity during incident window

## Causal Chain

- service_failure failure caused repeated 5xx responses
- Service instability propagated across dependent components
- This resulted in widespread failures across services: kubernetes-admin, system:kube-controller-manager, system:serviceaccount:cert-manager:my-cert-manager-startupapicheck, system:serviceaccount:gatekeeper-system:gatekeeper-admin, system:serviceaccount:kube-system:daemon-set-controller, system:serviceaccount:kube-system:generic-garbage-collector, system:serviceaccount:kube-system:job-controller, system:serviceaccount:kube-system:namespace-controller, system:serviceaccount:kube-system:replicaset-controller, system:serviceaccount:kube-system:resourcequota-controller, system:serviceaccount:kube-system:statefulset-controller


## Key Signals

- Confidence: high (0.99)
- Event count: 373.797582972583
- Error count: 373.797582972583
- Actor diversity: 12
- Control-plane impact: 11 patterns
- Trigger score: 3.029

## Primary Pattern

- Service: system:serviceaccount:cert-manager:my-cert-manager-cainjector
- Operation: get unknown
- Status: 5xx
- First seen: 2023-01-27T18:34:01.592519Z
- Last seen: 2023-01-27T18:44:08.381118Z

## Evidence

```
{"kind":"Event","apiVersion":"audit.k8s.io/v1","level":"Metadata","auditID":"d6825e56-7657-4455-9be7-7caa14b4ae6c","stage":"ResponseComplete","requestURI":"/apis/metrics.k8s.io/v1beta1?timeout=32s","verb":"get","user":{"username":"system:serviceaccount:cert-manager:my-cert-manager-cainjector","uid":"aaca50d4-b3f9-4fd1-9e8d-869fe253f70b","groups":["system:serviceaccounts","system:serviceaccounts:cert-manager","system:authenticated"],"extra":{"authentication.kubernetes.io/pod-name":["my-cert-manager-cainjector-6fc6455885-zgw9d"],"authentication.kubernetes.io/pod-uid":["799ed7ad-aa62-40ab-90a1-b1f3a19bceb1"]}},"sourceIPs":["192.168.60.12"],"userAgent":"cainjector/v0.0.0 (linux/amd64) kubernetes/$Format","responseStatus":{"metadata":{},"code":503},"requestReceivedTimestamp":"2023-01-27T18:34:01.592519Z","stageTimestamp":"2023-01-27T18:34:01.596947Z","annotations":{"authorization.k8s.io/decision":"allow","authorization.k8s.io/reason":"RBAC: allowed by ClusterRoleBinding \"system:discovery\" of ClusterRole \"system:discovery\" to Group \"system:authenticated\""}}
```

```
{"kind":"Event","apiVersion":"audit.k8s.io/v1","level":"Metadata","auditID":"67e16d50-c8e4-45b2-802d-12c5dab8cc17","stage":"ResponseComplete","requestURI":"/apis/metrics.k8s.io/v1beta1?timeout=32s","verb":"get","user":{"username":"system:serviceaccount:cert-manager:my-cert-manager-cainjector","uid":"aaca50d4-b3f9-4fd1-9e8d-869fe253f70b","groups":["system:serviceaccounts","system:serviceaccounts:cert-manager","system:authenticated"],"extra":{"authentication.kubernetes.io/pod-name":["my-cert-manager-cainjector-6fc6455885-zgw9d"],"authentication.kubernetes.io/pod-uid":["799ed7ad-aa62-40ab-90a1-b1f3a19bceb1"]}},"sourceIPs":["192.168.60.12"],"userAgent":"cainjector/v0.0.0 (linux/amd64) kubernetes/$Format","responseStatus":{"metadata":{},"code":503},"requestReceivedTimestamp":"2023-01-27T18:34:04.385773Z","stageTimestamp":"2023-01-27T18:34:04.386099Z","annotations":{"authorization.k8s.io/decision":"allow","authorization.k8s.io/reason":"RBAC: allowed by ClusterRoleBinding \"system:discovery\" of ClusterRole \"system:discovery\" to Group \"system:authenticated\""}}
```

```
{"kind":"Event","apiVersion":"audit.k8s.io/v1","level":"Metadata","auditID":"e1c7f02c-752b-47e8-9615-006c5ebb6211","stage":"ResponseComplete","requestURI":"/apis/metrics.k8s.io/v1beta1?timeout=32s","verb":"get","user":{"username":"system:serviceaccount:cert-manager:my-cert-manager-cainjector","uid":"aaca50d4-b3f9-4fd1-9e8d-869fe253f70b","groups":["system:serviceaccounts","system:serviceaccounts:cert-manager","system:authenticated"],"extra":{"authentication.kubernetes.io/pod-name":["my-cert-manager-cainjector-6fc6455885-zgw9d"],"authentication.kubernetes.io/pod-uid":["799ed7ad-aa62-40ab-90a1-b1f3a19bceb1"]}},"sourceIPs":["192.168.60.12"],"userAgent":"cainjector/v0.0.0 (linux/amd64) kubernetes/$Format","responseStatus":{"metadata":{},"code":503},"requestReceivedTimestamp":"2023-01-27T18:34:05.034886Z","stageTimestamp":"2023-01-27T18:34:05.035575Z","annotations":{"authorization.k8s.io/decision":"allow","authorization.k8s.io/reason":"RBAC: allowed by ClusterRoleBinding \"system:discovery\" of ClusterRole \"system:discovery\" to Group \"system:authenticated\""}}
```

## Alternative Hypotheses

- Authorization / RBAC failure (score=0.99, confidence=high)
