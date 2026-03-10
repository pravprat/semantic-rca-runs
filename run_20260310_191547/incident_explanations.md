# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 55.86

Root Cause: Gatekeeper resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C212, C28, C61, C21, C78

Blast Radius: 5


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 5

### Cluster C19

Behavior: kubernetes-admin get configmaps client failures (HTTP 404)

Score: 29.57

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:30:53.643535Z,kubernetes-admin,get,daemonsets,,my-prometheus-prometheus-node-exporter,,/apis/apps/v1/namespaces/prometheus/daemonsets/my-prometheus-prometheus-node-exporter,ce1a81bc-6a06-49f4-bfd5-00ef222f137d,ResponseComplete,404,,,

Propagation: C185, C28, C212, C61, C82

Blast Radius: 5


- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 128 events
- Error burst detected: 114 anomalous events
- Trigger proximity to incident start: 0.578
- Downstream clusters affected: 5

### Cluster C131

Behavior: Service account lookup failures

Score: 29.23

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:42.247463Z,system:apiserver,get,serviceaccounts,,policy-test-sa-1,,/api/v1/namespaces/kube-system/serviceaccounts/policy-test-sa-1,092c8dc0-0b71-45f3-9efd-cf534400e863,ResponseComplete,404,,,

Propagation: C28, C185, C212, C61, C49

Blast Radius: 5


- Behavior: system:apiserver get serviceaccounts (HTTP 404)
- Cluster size: 16 events
- Error burst detected: 16 anomalous events
- Trigger proximity to incident start: 0.69
- Downstream clusters affected: 5

### Cluster C165

Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)

Score: 28.43

Root Cause: Unknown Component normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:56.281482Z,kubernetes-admin,delete,rolebindings,,my-cert-manager-startupapicheck:create-cert,,/apis/rbac.authorization.k8s.io/v1/namespaces/cert-manager/rolebindings/my-cert-manager-startupapicheck:create-cert,bae1136b-888d-4fd1-b29a-a5f0bcbfed83,ResponseComplete,200,,,


Blast Radius: 0


- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 34 events
- Error burst detected: 28 anomalous events
- Trigger proximity to incident start: 0.028

### Cluster C111

Behavior: Node RBAC permission failures

Score: 26.95

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:43.254658Z,system:node:k8s-node-1-perfspec,list,configmaps,,my-airflow-airflow-config,,/api/v1/namespaces/default/configmaps?fieldSelector=metadata.name%3Dmy-airflow-airflow-config&resourceVersion=6135895,0a48a281-dd2c-4f7b-b35f-19b8adf82ab3,ResponseComplete,403,,,

Propagation: C185, C28, C212, C61, C82

Blast Radius: 5


- Behavior: system:node:k8s-node-1-perfspec list configmaps (HTTP 403)
- Cluster size: 6 events
- Error burst detected: 5 anomalous events
- Trigger proximity to incident start: 0.681
- Downstream clusters affected: 5

---
# Incident I2

### Cluster C0

Behavior: kubernetes-admin get configmaps client failures (HTTP 404)

Score: 50.41

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:06.032926Z,kubernetes-admin,get,rolebindings,,my-argo-cd-argocd-applicationset-controller,,/apis/rbac.authorization.k8s.io/v1/namespaces/argo-cd/rolebindings/my-argo-cd-argocd-applicationset-controller,ffb58937-bfd6-4945-b8d0-ce40f76d14ba,ResponseComplete,404,,,

Propagation: C185, C23, C162, C28, C16

Blast Radius: 5


- Behavior: kubernetes-admin get configmaps (HTTP 404)
- Cluster size: 90 events
- Error burst detected: 90 anomalous events
- Trigger proximity to incident start: 0.955
- Downstream clusters affected: 5

### Cluster C117

Behavior: k8s-node-1-perfspec patch events client failures (HTTP 404)

Score: 28.79

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:26.258728Z,system:node:k8s-node-1-perfspec,patch,events,,my-loki-logs-8mj42.173e3c8107533d12,,/api/v1/namespaces/loki/events/my-loki-logs-8mj42.173e3c8107533d12,cd45b930-0e98-4f16-a8e7-a20bd0704371,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:node:k8s-node-1-perfspec patch events (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.616

### Cluster C188

Behavior: kubernetes-admin get clusterroles client failures (HTTP 404)

Score: 27.08

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:43.341039Z,kubernetes-admin,get,rolebindings,,my-kubernetes-dashboard,,/apis/rbac.authorization.k8s.io/v1/namespaces/kubernetes-dashboard/rolebindings/my-kubernetes-dashboard,a1b98046-602c-48e2-9576-fcff631acd91,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: kubernetes-admin get clusterroles (HTTP 404)
- Cluster size: 4 events
- Error burst detected: 4 anomalous events
- Trigger proximity to incident start: 0.331

### Cluster C182

Behavior: Secret lookup failures

Score: 26.31

Root Cause: Unknown Component normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:20.098948Z,kubernetes-admin,create,secrets,,my-redis,,/api/v1/namespaces/redis/secrets?fieldManager=helm,70542958-e2f3-40e2-9ca1-6fd476f12d40,ResponseComplete,201,,,

Propagation: C185, C23, C14, C162, C28

Blast Radius: 5


- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733
- Downstream clusters affected: 5

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 21.87

Root Cause: Gatekeeper resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C212, C28, C61, C21, C78

Blast Radius: 5


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 5
