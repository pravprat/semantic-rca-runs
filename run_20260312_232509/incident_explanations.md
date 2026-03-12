# Semantic RCA Explanation Report

---
# Incident I1

### Cluster C1166

Behavior: mongodb activity

Score: 13.14

Root Cause: mongodb normal_operation

Trigger Event: [38;5;6mmongodb [38;5;5m00:05:09.74 [0m[38;5;2mINFO [0m ==> ** MongoDB Sharded setup finished! **

Propagation: C1006, C1058, C1080, C1083, C112, C1190, C128, C1280, C1342, C1349, C1444, C1455, C151, C1555, C1619, C1744, C1779, C179, C182, C1822, C1842, C1894, C305, C383, C39, C420, C48, C49, C490, C501, C521, C527, C532, C570, C590, C677, C70, C788, C800, C802, C853, C99

Blast Radius: 42


- Behavior: mongodb   (HTTP )
- Cluster size: 5 events
- Trigger proximity to incident start: 0.998
- Downstream clusters affected: 42

### Cluster C800

Behavior: mongodb activity

Score: 12.98

Root Cause: Unknown Component normal_operation

Trigger Event: Error receiving request from client. Ending connection from remote

Propagation: C1006, C1053, C1058, C1166, C1167, C1190, C128, C1308, C1367, C1403, C1423, C1555, C1619, C1744, C179, C1842, C1894, C305, C383, C39, C420, C48, C490, C521, C590, C677, C70, C788, C802, C853, C99

Blast Radius: 31


- Behavior: mongodb   (HTTP )
- Cluster size: 38 events
- Trigger proximity to incident start: 0.887
- Downstream clusters affected: 31

### Cluster C1006

Behavior: mongodb activity

Score: 11.83

Root Cause: Unknown Component normal_operation

Trigger Event: Connecting

Propagation: C1013, C1018, C1019, C1053, C1058, C108, C1083, C112, C1125, C116, C1166, C1167, C1190, C1251, C1253, C128, C1280, C1308, C1319, C1321, C1342, C1351, C1367, C1395, C1403, C1423, C1455, C1488, C1499, C1523, C154, C1555, C1561, C1563, C1609, C1619, C1632, C1639, C1640, C1669, C1677, C1697, C1715, C1727, C1731, C1744, C1753, C1779, C179, C180, C1816, C182, C1822, C1842, C185, C1894, C1911, C1928, C1939, C1955, C1971, C2012, C2014, C2023, C2029, C2034, C2044, C2077, C2109, C2149, C216, C2387, C2487, C281, C284, C305, C375, C381, C383, C39, C391, C417, C420, C427, C455, C48, C487, C49, C490, C51, C521, C524, C532, C590, C595, C677, C70, C76, C788, C800, C802, C815, C853, C858, C864, C871, C873, C941, C99

Blast Radius: 109


- Behavior: mongodb   (HTTP )
- Cluster size: 59 events
- Trigger proximity to incident start: 0.956
- Downstream clusters affected: 109

### Cluster C532

Behavior: mongodb activity

Score: 10.41

Root Cause: Unknown Component normal_operation

Trigger Event: timeout reached before the port went into state "inuse"

Propagation: C1006, C1053, C1058, C1083, C112, C1166, C1167, C1190, C1321, C1403, C1423, C1455, C1488, C154, C1677, C1731, C1744, C1753, C180, C1928, C2014, C305, C383, C39, C391, C417, C48, C490, C521, C524, C590, C677, C70, C788, C800, C802, C853, C873, C941, C99

Blast Radius: 40


- Behavior: mongodb   (HTTP )
- Cluster size: 39 events
- Trigger proximity to incident start: 0.753
- Downstream clusters affected: 40

### Cluster C677

Behavior: mongodb activity

Score: 9.69

Root Cause: Unknown Component normal_operation

Trigger Event: WiredTiger message

Propagation: C1006, C1053, C1058, C1083, C112, C1166, C1167, C1251, C128, C1280, C1321, C1403, C1423, C1455, C1488, C154, C1611, C1619, C1632, C1677, C1731, C1744, C1753, C1779, C180, C1822, C1842, C1894, C1911, C305, C39, C417, C420, C48, C49, C490, C521, C524, C532, C70, C788, C800, C802, C853, C873, C941, C99

Blast Radius: 47


- Behavior: mongodb   (HTTP )
- Cluster size: 19 events
- Trigger proximity to incident start: 0.827
- Downstream clusters affected: 47

---
# Incident I2

### Cluster C1619

Behavior: proxy activity

Score: 15.35

Root Cause: milvus normal_operation

Trigger Event: [2026/02/18 00:10:36.365 +00:00] [INFO] [resolver/resolver_with_discoverer.go:133] ["new grpc resolver registered"] [component=grpc-resolver] [scheme=milvus-session] [role=milvus/meta/session/rootcoord] [exclusive=true] [id=21]

Propagation: C1006, C1053, C1080, C1083, C1166, C1321, C1367, C1444, C1455, C1677, C1731, C1744, C1753, C179, C1842, C2012, C305, C381, C39, C427, C48, C490, C521, C590, C677, C70, C802, C941, C99

Blast Radius: 29


- Behavior: proxy   (HTTP )
- Cluster size: 61 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 29

### Cluster C1351

Behavior: proxy activity

Score: 12.09

Root Cause: Unknown Component normal_operation

Trigger Event: SIGNO: 11; SIGNAME: Segmentation fault; SI_CODE: 1; SI_ADDR: 0xa8

Propagation: C1125, C1340, C1744, C2077, C2109, C2387, C2487, C39, C48, C490, C99

Blast Radius: 11


- Behavior: proxy   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 0.959
- Downstream clusters affected: 11

### Cluster C2149

Behavior: proxy activity

Score: 12.09

Root Cause: Unknown Component normal_operation

Trigger Event: BACKTRACE:

Propagation: C1125, C1340, C1744, C2077, C2109, C2387, C2487, C39, C48, C490, C590, C99

Blast Radius: 12


- Behavior: proxy   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 0.959
- Downstream clusters affected: 12

### Cluster C2077

Behavior: proxy activity

Score: 11.98

Root Cause: Unknown Component normal_operation

Trigger Event: goroutine 289 gp=0xc000103c00 m=3 mp=0xc0000c9008 [running]:

Propagation: C1005, C1006, C1018, C1083, C112, C1125, C1166, C1167, C1223, C1321, C1340, C1624, C1673, C1677, C1731, C1744, C2071, C2109, C2251, C2284, C2312, C2387, C2487, C305, C356, C375, C383, C39, C420, C427, C455, C48, C482, C490, C521, C524, C590, C677, C70, C76, C788, C815, C853, C941, C99

Blast Radius: 45


- Behavior: proxy   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 0.902
- Downstream clusters affected: 45

### Cluster C2109

Behavior: proxy activity

Score: 11.98

Root Cause: Unknown Component normal_operation

Trigger Event: goroutine 3 gp=0xc000003340 m=nil [GC sweep wait]:

Propagation: C1005, C1006, C1018, C1083, C112, C1125, C1166, C1167, C1223, C1321, C1340, C1624, C1673, C1677, C1731, C1744, C2071, C2077, C2251, C2284, C2312, C2387, C2487, C305, C356, C375, C383, C39, C420, C427, C455, C48, C482, C490, C521, C524, C590, C677, C70, C76, C788, C815, C853, C941, C99

Blast Radius: 45


- Behavior: proxy   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 0.902
- Downstream clusters affected: 45

---
# Incident I3

### Cluster C1

Behavior: server activity

Score: 7.17

Root Cause: Unknown Component normal_operation

Trigger Event: 2026-02-18T00:11:30.802Z [ERROR] storage.raft: failed to appendEntries to: peer="{Voter cc796202-190e-52be-242d-2222d9293346 vault-2.vault-internal:8201}" error="msgpack decode error [pos 3536]: read tcp 10.42.173.159:43516->10.42.76.232:8201: i/o timeout"


Blast Radius: 0


- Behavior: server   (HTTP )
- Cluster size: 42 events
- Trigger proximity to incident start: 1.0

---
# Incident I4

### Cluster C146

Behavior: etcd activity

Score: 11.03

Root Cause: etcd normal_operation

Trigger Event: trace[1456590038] linearizableReadLoop

Propagation: C1167, C1319, C2077, C2109, C2387, C2487, C39, C48, C521, C590, C802, C99

Blast Radius: 12


- Behavior: etcd   (HTTP )
- Cluster size: 5 events
- Trigger proximity to incident start: 0.936
- Downstream clusters affected: 12

### Cluster C66

Behavior: etcd activity

Score: 7.71

Root Cause: etcd normal_operation

Trigger Event: failed to reach the peer URL


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 195 events
- Trigger proximity to incident start: 1.0

### Cluster C65

Behavior: etcd activity

Score: 7.71

Root Cause: etcd normal_operation

Trigger Event: failed to get version


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 195 events
- Trigger proximity to incident start: 1.0

### Cluster C2

Behavior: etcd activity

Score: 7.58

Root Cause: Unknown Component normal_operation

Trigger Event: dropped internal Raft message since sending buffer is full (overloaded network)


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 108 events
- Trigger proximity to incident start: 0.997

### Cluster C88

Behavior: etcd activity

Score: 6.52

Root Cause: etcd normal_operation

Trigger Event: storing new hash


Blast Radius: 0


- Behavior: etcd   (HTTP )
- Cluster size: 6 events
- Trigger proximity to incident start: 0.998

---
# Incident I5

### Cluster C929

Behavior: metrics activity

Score: 7.22

Root Cause: mongodb normal_operation

Trigger Event: time="2026-02-18T00:08:40Z" level=error msg="Cannot connect to MongoDB: cannot connect to MongoDB: server selection error: server selection timeout, current topology: { Type: Single, Servers: [{ Addr: localhost:27017, Type: Unknown, Last error: dial tcp [::1]:27017: connect: connection refused }, ] }"


Blast Radius: 0


- Behavior: metrics   (HTTP )
- Cluster size: 156 events
- Trigger proximity to incident start: 1.0

---
# Incident I6

### Cluster C1013

Behavior: utility activity

Score: 16.79

Root Cause: mongodb normal_operation

Trigger Event: 2026/02/18 00:10:14 Failed to connect to MongoDB: server selection error: context deadline exceeded, current topology: { Type: Unknown, Servers: [{ Addr: mongodb-sharded:27017, Type: Unknown, Last error: dial tcp 10.43.252.183:27017: connect: connection refused }, ] }

Propagation: C1080, C1166, C1444, C1744, C179, C383, C48, C490, C521, C527, C802, C99

Blast Radius: 12


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 12

### Cluster C358

Behavior: utility activity

Score: 13.65

Root Cause: Unknown Component normal_operation

Trigger Event: [job.JobService] Created gRPC connection to job-tracker:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)

Propagation: C0, C1013, C1080, C112, C1166, C1619, C1733, C1744, C179, C383, C39, C48, C490, C524, C527, C751, C788, C802, C99

Blast Radius: 19


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 19

### Cluster C933

Behavior: utility activity

Score: 13.65

Root Cause: Unknown Component normal_operation

Trigger Event: Waiting for HTTP server to be ready...

Propagation: C0, C1013, C1080, C112, C1166, C1619, C1733, C1744, C179, C383, C39, C48, C490, C524, C527, C751, C788, C802, C99

Blast Radius: 19


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 19

### Cluster C975

Behavior: utility activity

Score: 13.65

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server configured at ':8080' (probes only)

Propagation: C0, C1013, C1080, C112, C1166, C1619, C1733, C1744, C179, C383, C39, C48, C490, C524, C527, C751, C788, C802, C99

Blast Radius: 19


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 19

### Cluster C976

Behavior: utility activity

Score: 13.64

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server starting at ':8080'

Propagation: C1080, C112, C1166, C1744, C179, C39, C48, C490, C524, C527, C788, C802, C99

Blast Radius: 13


- Behavior: utility   (HTTP )
- Cluster size: 8 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 13

---
# Incident I7

### Cluster C1015

Behavior: policy-engine-chart activity

Score: 16.32

Root Cause: mongodb normal_operation

Trigger Event: 2026/02/18 00:04:52 Failed to connect to MongoDB: server selection error: context deadline exceeded, current topology: { Type: Unknown, Servers: [{ Addr: mongodb-sharded:27017, Type: Unknown, Last error: dial tcp 10.43.252.183:27017: connect: connection refused }, ] }

Propagation: C0, C1013, C1080, C112, C1166, C1619, C1733, C1744, C179, C383, C39, C48, C490, C524, C527, C751, C788, C802, C99

Blast Radius: 19


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 19

### Cluster C1089

Behavior: policy-engine-chart activity

Score: 14.0

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server starting at ':8080'

Propagation: C0, C1013, C1080, C1166, C1619, C1733, C1744, C179, C383, C39, C48, C490, C524, C527, C751, C802, C99

Blast Radius: 17


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 17

### Cluster C1058

Behavior: policy-engine-chart activity

Score: 13.99

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server is ready and accepting connections

Propagation: C1006, C1053, C1083, C1166, C1190, C1251, C1321, C1523, C1609, C1611, C1632, C1677, C1731, C1744, C179, C1842, C1894, C1911, C1931, C1955, C1971, C2012, C2023, C2034, C305, C381, C383, C39, C420, C48, C490, C521, C524, C532, C590, C677, C70, C788, C800, C802, C853, C941, C99

Blast Radius: 43


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 43

### Cluster C1110

Behavior: policy-engine-chart activity

Score: 8.74

Root Cause: Unknown Component normal_operation

Trigger Event: Initializing health probes


Blast Radius: 0


- Behavior: policy-engine-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C394

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

### Cluster C183

Behavior: metrics-server activity

Score: 7.19

Root Cause: dcn normal_operation

Trigger Event: E0218 00:06:24.533392       1 scraper.go:149] "Failed to scrape node" err="Get \"https://192.168.113.135:10250/metrics/resource\": dial tcp 192.168.113.135:10250: connect: connection refused" node="sti32-dcn-vsimrtp113-02"


Blast Radius: 0


- Behavior: metrics-server   (HTTP )
- Cluster size: 52 events
- Trigger proximity to incident start: 1.0

---
# Incident I9

### Cluster C648

Behavior: vector-store-chart activity

Score: 14.36

Root Cause: Unknown Component normal_operation

Trigger Event: S3Credentials retrieved successfully from k8s secret

Propagation: C1013, C1015, C1089, C358, C933, C975

Blast Radius: 6


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 6

### Cluster C1053

Behavior: vector-store-chart activity

Score: 13.28

Root Cause: Unknown Component normal_operation

Trigger Event: Metric Map successfully initialized with

Propagation: C1006, C1013, C1058, C1083, C112, C116, C1166, C1251, C1319, C1342, C1395, C1455, C1619, C1632, C1727, C1744, C179, C1822, C1894, C1911, C1964, C2077, C2109, C216, C2387, C2487, C281, C305, C383, C39, C417, C420, C48, C490, C521, C524, C532, C590, C677, C70, C800, C802, C853, C873, C99

Blast Radius: 45


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 45

### Cluster C1051

Behavior: vector-store-chart activity

Score: 13.06

Root Cause: Unknown Component normal_operation

Trigger Event: Health check endpoints registered

Propagation: C1013, C1015, C1089, C358, C933, C975

Blast Radius: 6


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 6

### Cluster C1087

Behavior: vector-store-chart activity

Score: 13.06

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server configured at ':8080' (probes only)

Propagation: C1013, C1015, C1089, C358, C933, C975

Blast Radius: 6


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 6

### Cluster C970

Behavior: vector-store-chart activity

Score: 13.06

Root Cause: milvus normal_operation

Trigger Event: Connecting to Milvus

Propagation: C1013, C1015, C1089, C358, C933, C975

Blast Radius: 6


- Behavior: vector-store-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0
- Downstream clusters affected: 6

---
# Incident I10

### Cluster C424

Behavior: metadata-chart activity

Score: 8.74

Root Cause: Unknown Component normal_operation

Trigger Event: [job.JobService] Created gRPC connection to job-tracker:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C1046

Behavior: metadata-chart activity

Score: 8.07

Root Cause: mongodb normal_operation

Trigger Event: 2026/02/18 00:08:38 Failed to connect to MongoDB: server selection error: context deadline exceeded, current topology: { Type: Unknown, Servers: [{ Addr: mongodb-sharded:27017, Type: Unknown, Last error: dial tcp 10.43.252.183:27017: connect: connection refused }, ] }


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C1022

Behavior: metadata-chart activity

Score: 7.05

Root Cause: Unknown Component normal_operation

Trigger Event: Waiting for HTTP server to be ready...


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C1090

Behavior: metadata-chart activity

Score: 7.05

Root Cause: Unknown Component normal_operation

Trigger Event: HTTP server is ready and accepting connections


Blast Radius: 0


- Behavior: metadata-chart   (HTTP )
- Cluster size: 7 events
- Trigger proximity to incident start: 1.0

### Cluster C1169

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

### Cluster C305

Behavior: ontap-monitor-chart activity

Score: 15.41

Root Cause: Unknown Component normal_operation

Trigger Event: Failed to connect to ONTAP AMQP: read tcp 10.42.7.217:32784->192.168.113.98:5668: read: connection reset by peer

Propagation: C1006, C1053, C1058, C1083, C112, C1251, C128, C1319, C1611, C1632, C1744, C182, C1842, C1894, C1911, C2023, C383, C39, C420, C48, C490, C521, C524, C590, C677, C70, C788, C802, C853, C99

Blast Radius: 30


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 38 events
- Trigger proximity to incident start: 0.991
- Downstream clusters affected: 30

### Cluster C1052

Behavior: ontap-monitor-chart activity

Score: 8.87

Root Cause: Unknown Component normal_operation

Trigger Event: Health check endpoints registered


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C1084

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: Initialized ONTAP Monitor Services


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C1085

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: Initialized SnapPubSub Service


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0

### Cluster C326

Behavior: ontap-monitor-chart activity

Score: 6.87

Root Cause: Unknown Component normal_operation

Trigger Event: [file-metadata.SnapshotMetadataService] Created gRPC connection to file-metadata:9090 with load balancing, keepalive (1m30s), and retry (max 10 attempts)


Blast Radius: 0


- Behavior: ontap-monitor-chart   (HTTP )
- Cluster size: 4 events
- Trigger proximity to incident start: 1.0
