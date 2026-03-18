# Incident I2

## Incident Window

2023-01-27T18:30:38.127428+00:00 → 2023-01-27T18:30:48.127428+00:00

## Root Cause

**Dominant failure domain**

A dominant failure domain was identified from the incident patterns. The earliest pattern is get nodes with status class 2xx.

## Why this is the Root Cause

- Earliest observed failure pattern in the incident window
- Affects multiple system actors (systemic impact)
- Impacts control-plane components
- High trigger intensity during incident window

The failure originates from `system:node:k8s-node-1-perfspec` performing `get nodes` operations resulting in `2xx` responses.

## Key Signals

- Confidence: high (0.84)
- Event count: 4525
- Error count: 0
- Actor diversity: 17
- Control-plane impact: 36 patterns
- Trigger score: 3.057

## Primary Pattern

- Service: system:node:k8s-node-1-perfspec
- Operation: get nodes
- Status: 2xx
- First seen: 2023-01-27T18:28:08.133757Z
- Last seen: 2023-01-27T18:32:02.160186Z

## Evidence

```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:08.133757Z,system:node:k8s-node-1-perfspec,get,nodes,,k8s-node-1-perfspec,,/api/v1/nodes/k8s-node-1-perfspec?resourceVersion=0&timeout=10s,ff9c2f51-23fc-4627-bbc8-36e1e563d747,ResponseComplete,200,,,
```

```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:18.396186Z,system:node:k8s-node-1-perfspec,get,nodes,,k8s-node-1-perfspec,,/api/v1/nodes/k8s-node-1-perfspec?resourceVersion=0&timeout=10s,9931fc76-d3b7-4f3c-aff3-c371b588c55a,ResponseComplete,200,,,
```

```
"{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:28.422254Z,system:node:k8s-node-1-perfspec,get,nodes,,k8s-node-1-perfspec,,/api/v1/nodes/k8s-node-1-perfspec?resourceVersion=0&timeout=10s,0b62a27b-e471-4464-8694-f2142500df8f,ResponseComplete,200,,,
```
