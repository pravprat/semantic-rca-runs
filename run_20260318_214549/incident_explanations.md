# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C65

Behavior: gatekeeper-admin list mutatorpodstatuses client failures (HTTP 404)

Score: 63.45

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:33.529423Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,mutatorpodstatuses,,,,/apis/status.gatekeeper.sh/v1beta1/mutatorpodstatuses?resourceVersion=6135954,ab64c043-a275-4c40-a81e-f39a4c546f1c,ResponseComplete,404,,,

Propagation: C129, C142, C175, C183, C185, C232, C244, C269, C46, C56, C7

Blast Radius: 11


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list mutatorpodstatuses (HTTP 404)
- Cluster size: 12 events
- Error burst detected: 12 anomalous events
- Trigger proximity to incident start: 0.637
- Downstream clusters affected: 11

### Cluster C56

Behavior: gatekeeper-admin list modifyset client failures (HTTP 404)

Score: 62.62

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:38.453815Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,modifyset,,,,/apis/mutations.gatekeeper.sh/v1/modifyset?resourceVersion=6135960,4ac7992b-7c4e-4de4-94bd-152f43555832,ResponseComplete,404,,,

Propagation: C129, C175, C183, C185, C227, C232, C236, C25, C34, C46, C7

Blast Radius: 11


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list modifyset (HTTP 404)
- Cluster size: 11 events
- Error burst detected: 11 anomalous events
- Trigger proximity to incident start: 0.567
- Downstream clusters affected: 11

### Cluster C117

Behavior: Secret lookup failures

Score: 41.81

Root Cause: my-kube-prometheus-stack-operator resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:11.213416Z,system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator,delete,secrets,,alertmanager-my-kube-prometheus-stack-alertmanager-tls-assets-1,,/api/v1/namespaces/kube-prometheus-stack/secrets/alertmanager-my-kube-prometheus-stack-alertmanager-tls-assets-1,72974e4e-e160-4d8b-aab3-8c1134417dc1,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator delete secrets (HTTP 404)
- Cluster size: 214 events
- Error burst detected: 214 anomalous events
- Trigger proximity to incident start: 0.099

### Cluster C72

Behavior: Gatekeeper policy evaluation failures

Score: 37.81

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:11.027814Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,constrainttemplates,,,,/apis/templates.gatekeeper.sh/v1beta1/constrainttemplates?resourceVersion=6135955,48196c66-2e15-4aa2-b24a-6c0a57dcb271,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list constrainttemplates (HTTP 404)
- Cluster size: 18 events
- Error burst detected: 18 anomalous events
- Trigger proximity to incident start: 0.959

### Cluster C71

Behavior: gatekeeper-admin list providers client failures (HTTP 404)

Score: 37.01

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:11.755148Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,providers,,,,/apis/externaldata.gatekeeper.sh/v1beta1/providers?resourceVersion=6135955,794caa3f-621c-4511-b964-40f4c03b8abf,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list providers (HTTP 404)
- Cluster size: 11 events
- Error burst detected: 11 anomalous events
- Trigger proximity to incident start: 0.948

---
# Incident I2

### Cluster C56

Behavior: gatekeeper-admin list modifyset client failures (HTTP 404)

Score: 28.22

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:38.453815Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,modifyset,,,,/apis/mutations.gatekeeper.sh/v1/modifyset?resourceVersion=6135960,4ac7992b-7c4e-4de4-94bd-152f43555832,ResponseComplete,404,,,

Propagation: C129, C175, C183, C185, C227, C232, C236, C25, C34, C46, C7

Blast Radius: 11


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list modifyset (HTTP 404)
- Cluster size: 11 events
- Error burst detected: 11 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 11

### Cluster C65

Behavior: gatekeeper-admin list mutatorpodstatuses client failures (HTTP 404)

Score: 27.82

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:33.529423Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,mutatorpodstatuses,,,,/apis/status.gatekeeper.sh/v1beta1/mutatorpodstatuses?resourceVersion=6135954,ab64c043-a275-4c40-a81e-f39a4c546f1c,ResponseComplete,404,,,

Propagation: C129, C142, C175, C183, C185, C232, C244, C269, C46, C56, C7

Blast Radius: 11


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list mutatorpodstatuses (HTTP 404)
- Cluster size: 12 events
- Error burst detected: 12 anomalous events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 11

### Cluster C117

Behavior: Secret lookup failures

Score: 22.76

Root Cause: my-kube-prometheus-stack-operator resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:29:11.213416Z,system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator,delete,secrets,,alertmanager-my-kube-prometheus-stack-alertmanager-tls-assets-1,,/api/v1/namespaces/kube-prometheus-stack/secrets/alertmanager-my-kube-prometheus-stack-alertmanager-tls-assets-1,72974e4e-e160-4d8b-aab3-8c1134417dc1,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:serviceaccount:kube-prometheus-stack:my-kube-prometheus-stack-operator delete secrets (HTTP 404)
- Cluster size: 214 events
- Error burst detected: 214 anomalous events
- Trigger proximity to incident start: 1.0

### Cluster C71

Behavior: gatekeeper-admin list providers client failures (HTTP 404)

Score: 17.88

Root Cause: gatekeeper-admin resource_lookup_failure

Trigger Event: "{""name"":""k8s-master-perfspec""}",2023-01-27T18:28:11.755148Z,system:serviceaccount:gatekeeper-system:gatekeeper-admin,list,providers,,,,/apis/externaldata.gatekeeper.sh/v1beta1/providers?resourceVersion=6135955,794caa3f-621c-4511-b964-40f4c03b8abf,ResponseComplete,404,,,


Blast Radius: 0


- Behavior: system:serviceaccount:gatekeeper-system:gatekeeper-admin list providers (HTTP 404)
- Cluster size: 11 events
- Error burst detected: 11 anomalous events
- Trigger proximity to incident start: 1.0
