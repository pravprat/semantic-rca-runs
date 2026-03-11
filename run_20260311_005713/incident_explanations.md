# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 87.14

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C157, C168, C200, C205, C21, C39, C57, C67, C75, C9, C96

Blast Radius: 11


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 11

### Cluster C67

Behavior: kubernetes-admin create services operations (HTTP 201)

Score: 46.04

Root Cause: argocd normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:07.397910Z,kubernetes-admin,create,deployments,,my-argo-cd-argocd-applicationset-controller,,/apis/apps/v1/namespaces/argo-cd/deployments?fieldManager=helm,2c957c9e-6b10-43b4-9326-e301a7866138,ResponseComplete,201,,,

Propagation: C112, C114, C125, C137, C168, C177, C191, C200, C21, C29, C39, C41, C44, C57, C87, C95, C96

Blast Radius: 17


- Behavior: kubernetes-admin create services (HTTP 201)
- Cluster size: 46 events
- Error burst detected: 9 anomalous events
- Trigger proximity to incident start: 0.575
- Downstream clusters affected: 17

### Cluster C165

Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)

Score: 36.12

Root Cause: Unknown Component normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:56.281482Z,kubernetes-admin,delete,rolebindings,,my-cert-manager-startupapicheck:create-cert,,/apis/rbac.authorization.k8s.io/v1/namespaces/cert-manager/rolebindings/my-cert-manager-startupapicheck:create-cert,bae1136b-888d-4fd1-b29a-a5f0bcbfed83,ResponseComplete,200,,,


Blast Radius: 0


- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 34 events
- Error burst detected: 28 anomalous events
- Trigger proximity to incident start: 0.028

### Cluster C19

Behavior: kubernetes-admin get configmaps client failures (HTTP 404)

Score: 32.13

Root Cause: prometheus resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:30:53.643535Z,kubernetes-admin,get,daemonsets,,my-prometheus-prometheus-node-exporter,,/apis/apps/v1/namespaces/prometheus/daemonsets/my-prometheus-prometheus-node-exporter,ce1a81bc-6a06-49f4-bfd5-00ef222f137d,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 128 events
- Error burst detected: 114 anomalous events
- Trigger proximity to incident start: 0.578

### Cluster C112

Behavior: kubernetes-admin delete clusterroles client failures (HTTP 404)

Score: 32.05

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:35.203282Z,kubernetes-admin,delete,rolebindings,,my-ingress-nginx-admission,,/apis/rbac.authorization.k8s.io/v1/namespaces/ingress-nginx/rolebindings/my-ingress-nginx-admission,764a853a-9228-4778-8a86-5548c5266591,ResponseComplete,404,,,

Propagation: C114, C168, C191, C200, C39, C57, C67

Blast Radius: 7


- Behavior: kubernetes-admin delete clusterroles (HTTP 404)
- Cluster size: 20 events
- Error burst detected: 12 anomalous events
- Trigger proximity to incident start: 0.216
- Downstream clusters affected: 7

---
# Incident I2

### Cluster C0

Behavior: kubernetes-admin get configmaps client failures (HTTP 404)

Score: 90.25

Root Cause: argocd resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:06.032926Z,kubernetes-admin,get,rolebindings,,my-argo-cd-argocd-applicationset-controller,,/apis/rbac.authorization.k8s.io/v1/namespaces/argo-cd/rolebindings/my-argo-cd-argocd-applicationset-controller,ffb58937-bfd6-4945-b8d0-ce40f76d14ba,ResponseComplete,404,,,

Propagation: C114, C125, C137, C168, C191, C200, C29, C57, C67, C87

Blast Radius: 10


- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 90 events
- Error burst detected: 90 anomalous events
- Trigger proximity to incident start: 0.955
- Downstream clusters affected: 10

### Cluster C117

Behavior: k8s-node-1-perfspec patch events client failures (HTTP 404)

Score: 38.54

Root Cause: loki resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:26.258728Z,system:node:k8s-node-1-perfspec,patch,events,,my-loki-logs-8mj42.173e3c8107533d12,,/api/v1/namespaces/loki/events/my-loki-logs-8mj42.173e3c8107533d12,cd45b930-0e98-4f16-a8e7-a20bd0704371,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:node:k8s-node-1-perfspec patch events (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.616

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 38.46

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C157, C168, C200, C205, C21, C39, C57, C67, C75, C9, C96

Blast Radius: 11


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 11

### Cluster C188

Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)

Score: 34.49

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:43.341039Z,kubernetes-admin,get,rolebindings,,my-kubernetes-dashboard,,/apis/rbac.authorization.k8s.io/v1/namespaces/kubernetes-dashboard/rolebindings/my-kubernetes-dashboard,a1b98046-602c-48e2-9576-fcff631acd91,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.331

### Cluster C182

Behavior: Secret lookup failures

Score: 30.36

Root Cause: redis normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:20.098948Z,kubernetes-admin,create,secrets,,my-redis,,/api/v1/namespaces/redis/secrets?fieldManager=helm,70542958-e2f3-40e2-9ca1-6fd476f12d40,ResponseComplete,201,,,


Blast Radius: 0


- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733
