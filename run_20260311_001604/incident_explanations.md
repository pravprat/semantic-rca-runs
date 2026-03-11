# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 59.86

Root Cause: gatekeeper resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C118, C152, C156, C161, C179, C18, C181, C187, C220, C36, C7, C96

Blast Radius: 12


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

### Cluster C31

Behavior: my-kube-prometheus-stack-operator get secrets operations (HTTP 200)

Score: 30.99

Root Cause: prometheus normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:12.022671Z,system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator,update,secrets,,prometheus-my-kube-prometheus-stack-prometheus,,/api/v1/namespaces/kube-prometheus-stack/secrets/prometheus-my-kube-prometheus-stack-prometheus,a8c7090c-c03f-429d-b2a7-0805a0e74172,ResponseComplete,200,,,

Propagation: C152, C156, C161, C169, C175, C181, C187, C220, C36, C47, C50, C7, C76, C77, C96

Blast Radius: 15


- Behavior: system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator get secrets (HTTP 200)
- Cluster size: 1343 events
- Error burst detected: 222 anomalous events
- Trigger proximity to incident start: 0.482
- Downstream clusters affected: 15

### Cluster C165

Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)

Score: 30.43

Root Cause: Unknown Component normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:56.281482Z,kubernetes-admin,delete,rolebindings,,my-cert-manager-startupapicheck:create-cert,,/apis/rbac.authorization.k8s.io/v1/namespaces/cert-manager/rolebindings/my-cert-manager-startupapicheck:create-cert,bae1136b-888d-4fd1-b29a-a5f0bcbfed83,ResponseComplete,200,,,


Blast Radius: 0


- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 34 events
- Error burst detected: 28 anomalous events
- Trigger proximity to incident start: 0.028

### Cluster C18

Behavior: kubernetes-admin create customresourcedefinitions client failures (HTTP 409)

Score: 28.45

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:47.909502Z,kubernetes-admin,create,customresourcedefinitions,,alertmanagerconfigs.monitoring.coreos.com,,/apis/apiextensions.k8s.io/v1/customresourcedefinitions?fieldManager=helm,68e32d5e-d001-4651-ae3c-00b45521c45b,ResponseComplete,409,,,

Propagation: C152, C156, C161, C175, C181, C187, C220, C31, C36, C50, C7, C76, C77, C96

Blast Radius: 14


- Behavior: kubernetes-admin create customresourcedefinitions (HTTP 409)
- Cluster size: 30 events
- Error burst detected: 17 anomalous events
- Trigger proximity to incident start: 0.676
- Downstream clusters affected: 14

### Cluster C19

Behavior: kubernetes-admin get configmaps client failures (HTTP 404)

Score: 27.11

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:30:53.643535Z,kubernetes-admin,get,daemonsets,,my-prometheus-prometheus-node-exporter,,/apis/apps/v1/namespaces/prometheus/daemonsets/my-prometheus-prometheus-node-exporter,ce1a81bc-6a06-49f4-bfd5-00ef222f137d,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 128 events
- Error burst detected: 114 anomalous events
- Trigger proximity to incident start: 0.578

---
# Incident I2

### Cluster C0

Behavior: kubernetes-admin get configmaps client failures (HTTP 404)

Score: 48.46

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:06.032926Z,kubernetes-admin,get,rolebindings,,my-argo-cd-argocd-applicationset-controller,,/apis/rbac.authorization.k8s.io/v1/namespaces/argo-cd/rolebindings/my-argo-cd-argocd-applicationset-controller,ffb58937-bfd6-4945-b8d0-ce40f76d14ba,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 90 events
- Error burst detected: 90 anomalous events
- Trigger proximity to incident start: 0.955

### Cluster C117

Behavior: k8s-node-1-perfspec patch events client failures (HTTP 404)

Score: 32.79

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:26.258728Z,system:node:k8s-node-1-perfspec,patch,events,,my-loki-logs-8mj42.173e3c8107533d12,,/api/v1/namespaces/loki/events/my-loki-logs-8mj42.173e3c8107533d12,cd45b930-0e98-4f16-a8e7-a20bd0704371,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:node:k8s-node-1-perfspec patch events (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.616

### Cluster C188

Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)

Score: 29.08

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:43.341039Z,kubernetes-admin,get,rolebindings,,my-kubernetes-dashboard,,/apis/rbac.authorization.k8s.io/v1/namespaces/kubernetes-dashboard/rolebindings/my-kubernetes-dashboard,a1b98046-602c-48e2-9576-fcff631acd91,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.331

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 27.87

Root Cause: gatekeeper resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C118, C152, C156, C161, C179, C18, C181, C187, C220, C36, C7, C96

Blast Radius: 12


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

### Cluster C182

Behavior: Secret lookup failures

Score: 25.97

Root Cause: Unknown Component normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:20.098948Z,kubernetes-admin,create,secrets,,my-redis,,/api/v1/namespaces/redis/secrets?fieldManager=helm,70542958-e2f3-40e2-9ca1-6fd476f12d40,ResponseComplete,201,,,


Blast Radius: 0


- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733
