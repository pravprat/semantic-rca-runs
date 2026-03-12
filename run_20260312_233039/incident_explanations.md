# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C1166

Behavior: mongodb activity

Score: 16.41

Root Cause: Unknown Component normal_operation

Trigger Event: Error receiving request from client. Ending connection from remote

Propagation: C1021, C1051, C1078, C1108, C1152, C1168, C1185, C1228, C1242, C1352, C1445, C1466, C1491, C1496, C151, C1557, C1703, C1719, C2, C213, C2203, C2212, C2268, C2306, C2344, C237, C2471, C2570, C275, C283, C355, C363, C38, C393, C402, C46, C499, C5, C500, C501, C536, C571, C592, C656, C68, C703, C724, C725, C728, C749, C770, C772, C773, C775, C78, C809, C864, C87, C893, C90, C915, C919, C923, C927, C944, C966

Blast Radius: 66


- Behavior: mongodb   (HTTP )
- Cluster size: 14 events
- Trigger proximity to incident start: 0.984
- Downstream clusters affected: 66

### Cluster C770

Behavior: mongodb activity

Score: 15.95

Root Cause: Unknown Component normal_operation

Trigger Event: Host failed in replica set

Propagation: C10, C100, C1021, C1025, C103, C1051, C1055, C1078, C1082, C1106, C1108, C1110, C1118, C1152, C1166, C1168, C1185, C1209, C121, C1228, C1237, C1242, C1243, C125, C1268, C1284, C1324, C1331, C1352, C1366, C1374, C1397, C1399, C1445, C146, C1466, C1468, C1489, C149, C1491, C1496, C151, C1512, C1518, C1557, C156, C1560, C1561, C1584, C16, C1603, C1612, C1638, C1664, C167, C1671, C1672, C1688, C1689, C170, C1702, C1703, C1714, C1719, C1733, C1736, C177, C184, C19, C1918, C1921, C1922, C1958, C1968, C1989, C1992, C1999, C2, C2016, C2036, C2039, C2052, C2053, C2058, C206, C2061, C2067, C2086, C213, C216, C2203, C2212, C226, C2268, C2306, C2344, C237, C239, C2471, C257, C2570, C275, C283, C301, C330, C331, C355, C363, C38, C387, C393, C402, C423, C46, C465, C499, C5, C500, C501, C520, C536, C552, C571, C580, C592, C597, C6, C608, C648, C656, C68, C681, C69, C703, C724, C725, C728, C733, C737, C749, C772, C773, C775, C78, C79, C798, C80, C809, C83, C857, C864, C87, C88, C890, C893, C90, C915, C919, C923, C927, C944, C953, C960, C966

Blast Radius: 164


- Behavior: mongodb   (HTTP )
- Cluster size: 1588 events
- Trigger proximity to incident start: 0.994
- Downstream clusters affected: 164

### Cluster C427

Behavior: mongodb activity

Score: 15.61

Root Cause: Unknown Component normal_operation

Trigger Event: Heartbeat failed after max retries

Propagation: C1078, C1166, C283, C387, C393, C5, C536, C608, C770, C772, C775, C87

Blast Radius: 12


- Behavior: mongodb   (HTTP )
- Cluster size: 778 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

### Cluster C681

Behavior: mongodb activity

Score: 14.71

Root Cause: Unknown Component normal_operation

Trigger Event: The ident was successfully dropped

Propagation: C10, C103, C1078, C1228, C1237, C1366, C146, C1518, C1560, C1561, C19, C2058, C213, C301, C331, C38, C465, C648, C725, C770, C772, C78, C809, C864, C890, C923, C960

Blast Radius: 27


- Behavior: mongodb   (HTTP )
- Cluster size: 14 events
- Trigger proximity to incident start: 0.992
- Downstream clusters affected: 27

### Cluster C1228

Behavior: mongodb activity

Score: 14.09

Root Cause: Unknown Component normal_operation

Trigger Event: Connection ended

Propagation: C10, C100, C1025, C103, C1051, C1055, C1078, C1106, C1152, C1166, C1168, C1185, C121, C1237, C1242, C1268, C1284, C1331, C1366, C1397, C1399, C146, C1466, C1496, C1512, C1518, C1560, C1561, C1638, C1672, C1688, C170, C19, C1918, C1921, C1922, C1968, C1989, C2036, C2039, C2053, C2058, C2061, C2067, C2086, C213, C2203, C226, C2306, C2344, C239, C257, C2570, C283, C301, C331, C363, C38, C387, C393, C46, C465, C499, C5, C500, C501, C520, C536, C592, C6, C608, C648, C656, C681, C703, C725, C733, C737, C749, C770, C772, C775, C78, C798, C809, C83, C857, C864, C87, C915, C919, C923, C927, C960

Blast Radius: 94


- Behavior: mongodb   (HTTP )
- Cluster size: 972 events
- Trigger proximity to incident start: 0.995
- Downstream clusters affected: 94

---
# Incident I2

### Cluster C2344

Behavior: proxy activity

Score: 13.32

Root Cause: Unknown Component normal_operation

Trigger Event: goroutine 5 gp=0xc000003dc0 m=nil [GC worker (idle), 10 minutes]:

Propagation: C1021, C1051, C1078, C1166, C1185, C1228, C1242, C1445, C1466, C1491, C1496, C151, C1557, C1664, C1702, C1703, C2, C213, C2203, C2212, C2268, C2306, C237, C2471, C2570, C275, C283, C38, C393, C46, C499, C5, C500, C536, C571, C580, C592, C656, C703, C724, C725, C749, C770, C772, C773, C78, C87, C893, C90, C915, C923, C927, C944, C966

Blast Radius: 54


- Behavior: proxy   (HTTP )
- Cluster size: 10 events
- Trigger proximity to incident start: 0.902
- Downstream clusters affected: 54

### Cluster C275

Behavior: proxy activity

Score: 12.47

Root Cause: milvus normal_operation

Trigger Event: all.logs: [1771373556.413668196, {"time":"2026-02-18T00:12:36.413668196Z","stream":"stderr","_p":"F","log":"","kubernetes":{"pod_name":"milvus-milvus-proxy-8d464b548-ns6vc","namespace_name":"aide-system","pod_id":"e6707083-0971-454f-8f38-2acc6ce64dc0","labels":{"app.kubernetes.io/component":"proxy","app.kubernetes.io/instance":"milvus","app.kubernetes.io/managed-by":"milvus-operator","app.kubernetes.io/name":"milvus","milvus.io/service":"true","pod-template-hash":"8d464b548"},"annotations":{"checksum/config":"d67acb2b1b11c614cfaa633c1d06d07386e08f37deb3397d4d812b83e8405430","cni.projectcalico.org/containerID":"415cd207ef835855482f515081572e875227251ebbbc8d035d4f739b404ceb30","cni.projectcalico.org/podIP":"10.42.173.135/32","cni.projectcalico.org/podIPs":"10.42.173.135/32","milvus.io/using-configmap":"milvus"},"host":"sti32-dcn-vsimrtp113-03","pod_ip":"10.42.173.135","container_name":"proxy","docker_id":"45252100a7db639187de3901193824c462c551743be6c2a61476fbf2b7f36fa1","container_hash":"sha256:81ebb625ec9f0671060e846bf6f609723be68e379a4bc5c19bc289f07ae82516","container_image":"docker.repo.eng.netapp.com/globalcicd/aidp/ai-data-platform/milvusdb/milvus:ntap-v2.5.11-51-cpu"}}]

Propagation: C1051, C1078, C1166, C1242, C1466, C1491, C1496, C1664, C1958, C2203, C2344, C283, C363, C393, C5, C500, C536, C592, C770, C772, C87, C923

Blast Radius: 22


- Behavior: proxy   (HTTP )
- Cluster size: 42 events
- Trigger proximity to incident start: 0.859
- Downstream clusters affected: 22

### Cluster C2570

Behavior: proxy activity

Score: 12.12

Root Cause: Unknown Component normal_operation

Trigger Event: 	/build/cmd/main.go:97 +0x24d fp=0xc001a55f50 sp=0xc001a55cd8 pc=0x53bad0d

Propagation: C1051, C1078, C1166, C1185, C1228, C1242, C1445, C1491, C151, C1557, C1664, C1702, C1703, C2, C213, C2203, C2212, C2268, C2306, C2344, C237, C283, C38, C393, C46, C499, C5, C500, C536, C571, C580, C592, C656, C703, C724, C725, C749, C770, C772, C773, C78, C87, C893, C90, C915, C923, C927, C944, C966

Blast Radius: 49


- Behavior: proxy   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 0.902
- Downstream clusters affected: 49

### Cluster C2471

Behavior: proxy activity

Score: 12.12

Root Cause: Unknown Component normal_operation

Trigger Event: 	/go/pkg/mod/golang.org/toolchain@v0.0.1-go1.24.1.linux-amd64/src/net/fd_posix.go:55 +0x25 fp=0xc001a17ca8 sp=0xc001a17c60 pc=0x20eda45

Propagation: C1051, C1166, C1185, C1445, C151, C1703, C2, C2203, C2344, C237, C2570, C38, C499, C500, C656, C703, C725, C770, C773, C78, C87, C90, C915, C927, C944

Blast Radius: 25


- Behavior: proxy   (HTTP )
- Cluster size: 36 events
- Trigger proximity to incident start: 0.902
- Downstream clusters affected: 25

### Cluster C2203

Behavior: proxy activity

Score: 12.12

Root Cause: Unknown Component normal_operation

Trigger Event: net.(*TCPListener).accept(0xc000fc7d40)

Propagation: C1021, C1051, C1078, C1166, C1185, C1228, C1242, C1445, C1466, C1491, C1496, C151, C1557, C1664, C1702, C1703, C2, C213, C2212, C2268, C2306, C2344, C237, C2471, C2570, C275, C283, C38, C393, C46, C499, C5, C500, C536, C571, C580, C592, C656, C703, C724, C725, C749, C770, C772, C773, C78, C87, C893, C90, C915, C923, C927, C944, C966

Blast Radius: 54


- Behavior: proxy   (HTTP )
- Cluster size: 24 events
- Trigger proximity to incident start: 0.902
- Downstream clusters affected: 54

---
# Incident I3

### Cluster C2

Behavior: server activity

Score: 17.75

Root Cause: Unknown Component normal_operation

Trigger Event: 2026-02-18T00:12:31.750Z [ERROR] storage.raft: failed to appendEntries to: peer="{Voter cc796202-190e-52be-242d-2222d9293346 vault-2.vault-internal:8201}" error="msgpack decode error [pos 3672]: read tcp 10.42.173.159:38978->10.42.76.232:8201: i/o timeout"

Propagation: C1078, C1166, C283, C387, C393, C5, C536, C608, C770, C772, C775, C87

Blast Radius: 12


- Behavior: server   (HTTP )
- Cluster size: 42 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

---
# Incident I4

### Cluster C80

Behavior: etcd activity

Score: 7.71

Root Cause: etcd normal_operation

Trigger Event: failed to reach the peer URL


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 195 events
- Trigger proximity to incident start: 1.0

### Cluster C79

Behavior: etcd activity

Score: 7.71

Root Cause: etcd normal_operation

Trigger Event: failed to get version


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 195 events
- Trigger proximity to incident start: 1.0

### Cluster C11

Behavior: etcd activity

Score: 7.58

Root Cause: Unknown Component normal_operation

Trigger Event: dropped internal Raft message since sending buffer is full (overloaded network)


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 108 events
- Trigger proximity to incident start: 0.997

### Cluster C114

Behavior: etcd activity

Score: 6.52

Root Cause: etcd normal_operation

Trigger Event: storing new hash


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 6 events
- Trigger proximity to incident start: 0.998

### Cluster C115

Behavior: etcd activity

Score: 6.06

Root Cause: etcd normal_operation

Trigger Event: sending database snapshot to client


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 0.998

---
# Incident I5

### Cluster C1078

Behavior: metrics activity

Score: 17.8

Root Cause: mongodb normal_operation

Trigger Event: time="2026-02-18T00:06:36Z" level=error msg="Cannot connect to MongoDB: cannot connect to MongoDB: server selection error: server selection timeout, current topology: { Type: Single, Servers: [{ Addr: localhost:27017, Type: Unknown, Last error: dial tcp [::1]:27017: connect: connection refused }, ] }"

Propagation: C10, C100, C1021, C1025, C103, C1051, C1055, C1106, C1110, C1118, C1152, C1166, C1168, C1185, C1209, C121, C1228, C1237, C1242, C125, C1268, C1284, C1324, C1331, C1352, C1366, C1374, C1397, C1399, C1445, C146, C1466, C1468, C1489, C1496, C1512, C1518, C156, C1560, C1561, C1638, C1664, C167, C1671, C1672, C1688, C170, C1714, C177, C19, C1918, C1922, C1958, C1968, C1989, C2016, C2036, C2039, C2052, C2053, C2058, C206, C2061, C2086, C213, C2203, C226, C2268, C2344, C2471, C2570, C275, C283, C301, C330, C331, C355, C363, C38, C387, C393, C423, C46, C465, C499, C5, C500, C501, C520, C536, C552, C580, C592, C608, C648, C656, C681, C69, C703, C725, C728, C733, C737, C749, C770, C772, C775, C78, C79, C798, C80, C809, C83, C857, C864, C87, C88, C890, C90, C915, C919, C923, C927, C953, C960

Blast Radius: 125


- Behavior: metrics   (HTTP )
- Cluster size: 156 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 125

---
# Incident I6

### Cluster C1146

Behavior: utility activity

Score: 16.92

Root Cause: mongodb normal_operation

Trigger Event: 2026/02/18 00:10:14 Failed to connect to MongoDB: server selection error: context deadline exceeded, current topology: { Type: Unknown, Servers: [{ Addr: mongodb-sharded:27017, Type: Unknown, Last error: dial tcp 10.43.252.183:27017: connect: connection refused }, ] }

Propagation: C1166, C213, C283, C387, C393, C5, C536, C608, C770, C772, C775, C87

Blast Radius: 12


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

### Cluster C406

Behavior: utility activity

Score: 13.77

Root Cause: Unknown Component normal_operation

Trigger Event: [job.JobService] Created gRPC connection to job-tracker:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)

Propagation: C1078, C1146, C1166, C1242, C1363, C2, C213, C241, C283, C301, C387, C393, C427, C442, C5, C536, C608, C728, C770, C772, C87

Blast Radius: 21


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 21

### Cluster C815

Behavior: utility activity

Score: 13.77

Root Cause: Unknown Component normal_operation

Trigger Event: Waiting for HTTP server to be ready...

Propagation: C1166, C1242, C213, C283, C301, C393, C5, C536, C608, C728, C770, C772, C87

Blast Radius: 13


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 13

### Cluster C842

Behavior: utility activity

Score: 13.77

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server configured at ':8080' (probes only)

Propagation: C1078, C1146, C1166, C1242, C1363, C2, C213, C241, C283, C301, C387, C393, C427, C442, C5, C536, C608, C728, C770, C772, C87

Blast Radius: 21


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 21

### Cluster C843

Behavior: utility activity

Score: 13.77

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server starting at ':8080'

Propagation: C1166, C1242, C213, C283, C301, C393, C5, C536, C608, C728, C770, C772, C87

Blast Radius: 13


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 13

---
# Incident I7

### Cluster C1028

Behavior: policy-engine-chart activity

Score: 15.42

Root Cause: Unknown Component normal_operation

Trigger Event: Initializing health probes

Propagation: C1078, C1146, C1166, C1363, C2, C213, C241, C283, C387, C393, C427, C442, C536, C608, C770, C87

Blast Radius: 16


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 16

### Cluster C961

Behavior: policy-engine-chart activity

Score: 14.13

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server starting at ':8080'

Propagation: C1078, C1146, C1166, C1363, C2, C213, C241, C283, C387, C393, C427, C442, C536, C608, C770, C87

Blast Radius: 16


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 16

### Cluster C960

Behavior: policy-engine-chart activity

Score: 13.42

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server configured at ':8080' (probes only)

Propagation: C10, C100, C1051, C1078, C1146, C1152, C1166, C1168, C1185, C1228, C1237, C1242, C125, C1324, C1331, C1363, C1366, C1374, C146, C1489, C1512, C1584, C1603, C1612, C1638, C1688, C170, C177, C19, C1918, C1989, C1999, C2, C2036, C2039, C2058, C213, C241, C283, C301, C330, C38, C387, C393, C423, C427, C442, C46, C465, C499, C500, C501, C536, C580, C592, C608, C648, C656, C681, C703, C725, C770, C772, C775, C78, C79, C798, C80, C809, C857, C864, C87, C890, C915, C919, C923, C927

Blast Radius: 77


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 77

### Cluster C1148

Behavior: policy-engine-chart activity

Score: 8.07

Root Cause: mongodb normal_operation

Trigger Event: 2026/02/18 00:04:52 Failed to connect to MongoDB: server selection error: context deadline exceeded, current topology: { Type: Unknown, Servers: [{ Addr: mongodb-sharded:27017, Type: Unknown, Last error: dial tcp 10.43.252.183:27017: connect: connection refused }, ] }


Blast Radius: 0


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C428

Behavior: policy-engine-chart activity

Score: 7.05

Root Cause: Unknown Component normal_operation

Trigger Event: [job.JobService] Created gRPC connection to job-tracker:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)


Blast Radius: 0


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

---
# Incident I8

### Cluster C66

Behavior: metrics-server activity

Score: 7.19

Root Cause: dcn normal_operation

Trigger Event: E0218 00:08:54.532825       1 scraper.go:149] "Failed to scrape node" err="Get \"https://192.168.113.135:10250/metrics/resource\": dial tcp 192.168.113.135:10250: connect: connection refused" node="sti32-dcn-vsimrtp113-02"


Blast Radius: 0


- Behavior: metrics-server   (HTTP )
- Cluster size: 52 events
- Trigger proximity to incident start: 1.0

---
# Incident I9

### Cluster C809

Behavior: vector-store-chart activity

Score: 14.13

Root Cause: mongodb normal_operation

Trigger Event: Initializing vector store services (Milvus, MongoDB, etc.)

Propagation: C10, C100, C1051, C1078, C1152, C1166, C1168, C1228, C1237, C1242, C1331, C1374, C170, C1733, C177, C1918, C1922, C1992, C2053, C213, C2203, C2344, C2570, C283, C301, C38, C387, C402, C423, C46, C465, C500, C501, C580, C648, C68, C69, C725, C728, C733, C770, C772, C775, C78, C857, C87, C919, C923, C960

Blast Radius: 49


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 49

### Cluster C864

Behavior: vector-store-chart activity

Score: 14.13

Root Cause: Unknown Component normal_operation

Trigger Event: Waiting for HTTP server to be ready...

Propagation: C10, C100, C1051, C1078, C1106, C1152, C1166, C1168, C1228, C1237, C1242, C1331, C1374, C170, C1733, C177, C19, C1918, C1922, C1968, C1992, C2053, C206, C213, C2203, C2344, C2570, C283, C301, C330, C38, C387, C402, C423, C46, C465, C500, C501, C520, C580, C608, C648, C68, C69, C725, C728, C733, C770, C772, C775, C78, C79, C80, C857, C87, C919, C923, C960

Blast Radius: 58


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 58

### Cluster C890

Behavior: vector-store-chart activity

Score: 14.13

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server is ready and accepting connections

Propagation: C10, C1028, C1146, C1152, C1228, C1237, C1242, C1918, C213, C301, C38, C406, C501, C648, C733, C770, C775, C78, C842, C857, C87, C919, C960, C961

Blast Radius: 24


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 24

### Cluster C958

Behavior: vector-store-chart activity

Score: 13.17

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server starting at ':8080'

Propagation: C1028, C1146, C406, C842, C960, C961

Blast Radius: 6


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 6

### Cluster C959

Behavior: vector-store-chart activity

Score: 13.17

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server configured at ':8080' (probes only)

Propagation: C1028, C1146, C406, C842, C960, C961

Blast Radius: 6


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 6

---
# Incident I10

### Cluster C923

Behavior: metadata-chart activity

Score: 14.13

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server is ready and accepting connections

Propagation: C10, C100, C1025, C1051, C1078, C1082, C1106, C1108, C1118, C1152, C1166, C1168, C1209, C1228, C1237, C125, C1284, C1324, C1331, C1397, C1512, C16, C1603, C1664, C1702, C1719, C1736, C19, C1918, C1922, C1958, C1968, C1999, C2016, C2036, C2039, C2052, C2053, C213, C2203, C226, C2344, C2471, C257, C2570, C283, C301, C38, C387, C393, C46, C465, C5, C500, C501, C520, C536, C580, C6, C68, C703, C725, C728, C737, C770, C772, C775, C78, C809, C857, C864, C87, C890, C919, C960

Blast Radius: 75


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 75

### Cluster C1079

Behavior: metadata-chart activity

Score: 13.42

Root Cause: Unknown Component normal_operation

Trigger Event: Initializing health probes

Propagation: C1166, C1168, C213, C2203, C2344, C2570, C5, C501, C703, C770, C772, C87

Blast Radius: 12


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

### Cluster C455

Behavior: metadata-chart activity

Score: 8.74

Root Cause: Unknown Component normal_operation

Trigger Event: [job.JobService] Created gRPC connection to job-tracker:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C1171

Behavior: metadata-chart activity

Score: 8.07

Root Cause: mongodb normal_operation

Trigger Event: 2026/02/18 00:08:38 Failed to connect to MongoDB: server selection error: context deadline exceeded, current topology: { Type: Unknown, Servers: [{ Addr: mongodb-sharded:27017, Type: Unknown, Last error: dial tcp 10.43.252.183:27017: connect: connection refused }, ] }


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C1031

Behavior: metadata-chart activity

Score: 7.05

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server starting at ':8080'


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

---
# Incident I11

### Cluster C957

Behavior: ontap-monitor-chart activity

Score: 8.87

Root Cause: Unknown Component normal_operation

Trigger Event: Health check endpoints registered


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C373

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: [file-metadata.SnapshotMetadataService] Created gRPC connection to file-metadata:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C557

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: Initialized gRPC client to Snapshot Metadata Service


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C841

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: Initialized SnapPubSub Service


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C920

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: Initialized ONTAP Monitor Services


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0
