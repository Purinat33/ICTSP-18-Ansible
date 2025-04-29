## SITE A

**Servers**: 1
**Indexers**: 1
**Agents**: 1
**LoadBalancers**: 0

### Server Cluster:
- **server_a_1**
  - IP: 192.168.79.50
  - Role: MASTER

### Indexers
- **indexer_a_1**
  - IP: 192.168.79.55

### Agents
- **agent_a_1**
  - IP: 192.168.79.60

### Load Balancers

## SITE B

**Servers**: 1
**Indexers**: 1
**Agents**: 1
**LoadBalancers**: 0

### Server Cluster:
- **server_b_3**
  - IP: 192.168.97.52
  - Role: MASTER

### Indexers
- **indexer_b_1**
  - IP: 192.168.97.55

### Agents
- **agent_b_1**
  - IP: 192.168.97.60

### Load Balancers


## Global Load Balancer (`opensearch.hosts`)
["https://192.168.79.55:9200", "https://192.168.97.55:9200"]
