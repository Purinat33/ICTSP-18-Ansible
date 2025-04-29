## SITE A

**Servers**: 2
**Indexers**: 1
**Agents**: 1
**LoadBalancers**: 1

### Server Cluster:
- **server_a_1**
  - IP: 192.168.133.22
  - Role: MASTER
- **server_a_2**
  - IP: 192.168.133.26
  - Role: WORKER

### Indexers
- **indexer_a_1**
  - IP: 192.168.133.21

### Agents
- **agent_a_1**
  - IP: 192.168.133.23

### Load Balancers
- **lb_a_1**
  - IP: 192.168.133.25

## SITE B

**Servers**: 3
**Indexers**: 2
**Agents**: 2
**LoadBalancers**: 1

### Server Cluster:
- **server_b_1**
  - IP: 192.168.234.6
  - Role: MASTER
- **server_b_2**
  - IP: 192.168.234.100
  - Role: WORKER
- **server_b_3**
  - IP: 192.168.234.200
  - Role: WORKER

### Indexers
- **indexer_b_1**
  - IP: 192.168.234.5
- **indexer_b_2**
  - IP: 192.168.234.100

### Agents
- **agent_b_1**
  - IP: 192.168.234.8
- **agent_b_2**
  - IP: 192.168.234.18

### Load Balancers
- **lb_b_1**
  - IP: 192.168.234.199

## SITE C

**Servers**: 1
**Indexers**: 1
**Agents**: 1
**LoadBalancers**: 0

### Server Cluster:
- **server_c_1**
  - IP: 192.168.1.3
  - Role: MASTER

### Indexers
- **indexer_c_1**
  - IP: 192.168.1.2

### Agents
- **agent_c_1**
  - IP: 192.168.1.4

### Load Balancers


## Global Load Balancer (`opensearch.hosts`)
["https://192.168.133.21:9200", "https://192.168.234.5:9200", "https://192.168.234.100:9200", "https://192.168.1.2:9200"]
