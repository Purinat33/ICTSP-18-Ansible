## SITE A

**Servers**: 2
**Indexers**: 1
**Agents**: 2
**LoadBalancers**: 1

### Server Cluster:
- **server_a_1**
  - IP: 192.168.79.50
  - Role: MASTER
- **server_a_2**
  - IP: 192.168.79.51
  - Role: WORKER

### Indexers
- **indexer_a_1**
  - IP: 192.168.79.55

### Agents
- **agent_a_1**
  - IP: 192.168.79.60
- **agent_a_2**
  - IP: 192.168.79.70

### Load Balancers
- **lb_a_1**
  - IP: 192.168.79.199

## SITE B

**Servers**: 3
**Indexers**: 2
**Agents**: 1
**LoadBalancers**: 1

### Server Cluster:
- **server_b_3**
  - IP: 192.168.97.52
  - Role: MASTER
- **server_b_4**
  - IP: 192.168.97.98
  - Role: WORKER
- **server_b_5**
  - IP: 192.168.97.97
  - Role: WORKER

### Indexers
- **indexer_b_1**
  - IP: 192.168.97.55
- **indexer_b_2**
  - IP: 192.168.97.100

### Agents
- **agent_b_1**
  - IP: 192.168.97.60

### Load Balancers
- **lb_b_1**
  - IP: 192.168.97.200


## Global Load Balancer (`opensearch.hosts`)
["https://192.168.79.55:9200", "https://192.168.97.55:9200", "https://192.168.97.100:9200"]
