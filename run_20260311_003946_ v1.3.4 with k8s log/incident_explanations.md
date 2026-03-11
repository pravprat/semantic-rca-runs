# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 73.0

Root Cause: gatekeeper resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C1, C11, C155, C157, C187, C2, C4, C65

Blast Radius: 8


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 8

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

### Cluster C112

Behavior: kubernetes-admin delete clusterroles client failures (HTTP 404)

Score: 23.96

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:35.203282Z,kubernetes-admin,delete,rolebindings,,my-ingress-nginx-admission,,/apis/rbac.authorization.k8s.io/v1/namespaces/ingress-nginx/rolebindings/my-ingress-nginx-admission,764a853a-9228-4778-8a86-5548c5266591,ResponseComplete,404,,,

Propagation: C1, C157, C187, C65, C76

Blast Radius: 5


- Behavior: kubernetes-admin delete clusterroles (HTTP 404)
- Cluster size: 20 events
- Error burst detected: 12 anomalous events
- Trigger proximity to incident start: 0.216
- Downstream clusters affected: 5

### Cluster C111

Behavior: Node RBAC permission failures

Score: 23.05

Root Cause: Unknown Component resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:43.254658Z,system:node:k8s-node-1-perfspec,list,configmaps,,my-airflow-airflow-config,,/api/v1/namespaces/default/configmaps?fieldSelector=metadata.name%3Dmy-airflow-airflow-config&resourceVersion=6135895,0a48a281-dd2c-4f7b-b35f-19b8adf82ab3,ResponseComplete,403,,,


Blast Radius: 0


- Behavior: system:node:k8s-node-1-perfspec list configmaps (HTTP 403)
- Cluster size: 6 events
- Error burst detected: 5 anomalous events
- Trigger proximity to incident start: 0.681

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

### Cluster C182

Behavior: Secret lookup failures

Score: 38.27

Root Cause: Unknown Component normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:20.098948Z,kubernetes-admin,create,secrets,,my-redis,,/api/v1/namespaces/redis/secrets?fieldManager=helm,70542958-e2f3-40e2-9ca1-6fd476f12d40,ResponseComplete,201,,,

Propagation: C1, C101, C15, C157, C187, C58

Blast Radius: 6


- Behavior: kubernetes-admin get secrets (HTTP 404)
- Cluster size: 27 events
- Error burst detected: 13 anomalous events
- Trigger proximity to incident start: 0.733
- Downstream clusters affected: 6

### Cluster C15

Behavior: argocd-applicationset-controller get secrets operations (HTTP 200)

Score: 35.94

Root Cause: argocd normal_operation

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:31:09.870252Z,system:serviceaccount:argo-cd:argocd-application-controller,list,secrets,,,,/api/v1/namespaces/argo-cd/secrets?labelSelector=argocd.argoproj.io%2Fsecret-type%3Dcluster&limit=500&resourceVersion=0,c2e3100c-863b-4597-8e28-d0ad45091e1e,ResponseComplete,200,,,

Propagation: C1, C101, C157, C182, C187, C58

Blast Radius: 6


- Behavior: system:serviceaccount:argo-cd:argocd-applicationset-controller get secrets (HTTP 200)
- Cluster size: 99 events
- Error burst detected: 23 anomalous events
- Trigger proximity to incident start: 0.951
- Downstream clusters affected: 6

### Cluster C163

Behavior: Gatekeeper policy evaluation failures

Score: 33.12

Root Cause: gatekeeper resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:22.470778Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,assignmetadata,,,,/apis/mutations.gatekeeper.sh/v1/assignmetadata?resourceVersion=6135961,2c893351-f825-40f8-9bf7-19ff1de0fb4f,ResponseComplete,404,,,

Propagation: C1, C11, C155, C157, C187, C2, C4, C65

Blast Radius: 8


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 112 events
- Error burst detected: 108 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 8

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
