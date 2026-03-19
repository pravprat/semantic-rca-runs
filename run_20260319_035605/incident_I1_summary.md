# Incident I1

## Incident Window

2023-01-27T18:28:08.127428+00:00 → 2023-01-27T18:32:18.127428+00:00

## Root Cause

**Authorization / RBAC failure**

Repeated authorization failures were detected. The earliest pattern is watch configmaps with 4xx. The failure affects 5 actor(s), including 7 control-plane pattern(s).

## Why this is the Root Cause

- Earliest observed failure pattern in the incident window
- Affects multiple system actors (systemic impact)
- Impacts control-plane components
- Consistent authorization/client error responses
- High trigger intensity during incident window

## Causal Chain

- authz failure triggered 4xx responses
- system:node:k8s-node-1-perfspec experienced 4xx errors
- system:kube-scheduler experienced 4xx errors
- system:node:k8s-node-2-perfspec experienced 4xx errors


## Key Signals

- Confidence: high (0.99)
- Event count: 21.457142857142856
- Error count: 21.457142857142856
- Actor diversity: 5
- Control-plane impact: 7 patterns
- Trigger score: 3.413

## Primary Pattern

- Service: system:node:k8s-node-1-perfspec
- Operation: watch configmaps
- Status: 4xx
- First seen: 2023-01-27T18:28:08.129781Z
- Last seen: 2023-01-27T18:28:08.135575Z

## Evidence

```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:08.129781Z,system:node:k8s-node-1-perfspec,watch,configmaps,,kube-flannel-cfg,,/api/v1/namespaces/kube-flannel/configmaps?allowWatchBookmarks=true&fieldSelector=metadata.name%3Dkube-flannel-cfg&resourceVersion=6577334&timeout=7m43s&timeoutSeconds=463&watch=true,a1b86d5d-6f8f-4058-9710-19f5cc40a68a,ResponseStarted,403,,,
```

```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:08.131024Z,system:node:k8s-node-1-perfspec,watch,configmaps,,kube-root-ca.crt,,/api/v1/namespaces/kube-system/configmaps?allowWatchBookmarks=true&fieldSelector=metadata.name%3Dkube-root-ca.crt&resourceVersion=6577334&timeout=6m5s&timeoutSeconds=365&watch=true,b51f1a8c-e53e-4104-b1a6-e695a24ed43c,ResponseStarted,403,,,
```

```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:08.130396Z,system:node:k8s-node-1-perfspec,watch,configmaps,,kube-proxy,,/api/v1/namespaces/kube-system/configmaps?allowWatchBookmarks=true&fieldSelector=metadata.name%3Dkube-proxy&resourceVersion=6577334&timeout=6m21s&timeoutSeconds=381&watch=true,3ba9cc6d-7d10-40c5-8ec7-da60a9b3627c,ResponseComplete,403,,,
```
