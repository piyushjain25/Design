# System Design Interview

Questions to be asked to interviewer to finalize the MVP for the interview
1. **Features**
2. **API**
3. **Availability** - Single Point of Failure, etc
4. **Latency / Performance** - Backend job or Customer facing. Consider Caching and stuff.
5. **Scalability** - Work for 100 / 1000 / Million users? Should the design scale as user increases?
6. **Durability** - Data storage i.e. Database. Design a database model as well or just use any existing one?
7. **Class Diagram** - Object Oriented Principles
8. **Security and Privacy** 
9. **Cost-effective** - Pros & Cons of different solution and any alternate cost effective solution.


# All the concepts to improve system design problem solving

### 1. Vertical vs horizontal scaling
  Vertical - Adding memory/CPU onto the existing system - Expensive and limitation on how much you can add to an existing system.
  Horizontal - Infinitely keep adding multiple hosts introducing distributed system challenges.
  
### 2. CAP theorem
  We can have 2 out of the 3.
  Consistency - Read has the most recent writes
  Availability - Data is available all the time i.e. most recent data is available whenever you read.
  Partition Tolerance - There may be package drops between multiple nodes.
  
  Relational DBs are Consistent over Available
  NoSQL DBs prefer Availability over Consistency if configured that way.
  
### 3. ACID vs BASE

### 4. Partitioning/Sharding 

### 5. Consistent Hashing

### 6. Optimistic vs pessimistic locking

### 7. Strong vs eventual consistency

### 8. RelationalDB vs NoSQL

### 9. Types of NoSQL
     Key value
     Wide column
     Document-based
     Graph-based

### 10. Caching

### 11. Data center/racks/hosts

### 12. CPU/memory/Hard drives/Network bandwidth

### 13. Random vs sequential read/writes to disk

### 14. HTTP vs http2 vs WebSocket

### 15. TCP/IP model

### 16. ipv4 vs ipv6

### 17. TCP vs UDP

### 18. DNS lookup

### 19. Http & TLS

### 20. Public key infrastructure and certificate authority(CA)

### 21. Symmetric vs asymmetric encryption

### 22. Load Balancer

### 23. CDNs & Edges

### 24. Bloom filters and Count-Min sketch

### 25. Paxos 

### 26. Leader election

### 27. Design patterns and Object-oriented design

### 28. Virtual machines and containers

### 29. Pub-sub architecture 

### 30. MapReduce

### 31. Multithreading, locks, synchronization, CAS(compare and set)


# Tools

1. Cassandra
2. MongoDB/Couchbase
3. Mysql
4. Memcached
5. Redis
6. Zookeeper
7. Kafka
8. NGINX
9. HAProxy
10. Solr, Elastic search
11. Amazon S3
12. Docker, Kubernetes, Mesos
13. Hadoop/Spark and HDFS
