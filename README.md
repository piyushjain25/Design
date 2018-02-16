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
  Atomicity, Consistency, Isolation, Durability (More for traditional SQL DBs)
  Basically Available Soft state Eventual Consistency (Modern NoSQL DBs)

### 4. Partitioning / Sharding
  Sharding - Splitting data across nodes/system to accomodate tons of millions of data
  Sharding technique - Consistent Hashing

### 6. Optimistic vs Pessimistic Locking
  Optimistic Locking - With no locks acquired, at the time of commiting the changes, we check if no other transaction updated the records.
  Pessimistic Locking - Acquire locks before hand and then commit the transaction.
  
  More on advantages/disadvantages and understanding which one to use in which scenario.

### 7. Strong vs Eventual consistency
  Strong - Reads will always see latest writes (Relational DB)
  Eventual - Reads will see some writes and eventually in some time, it will see all the writes (NoSql can be configured either ways)

### 8. Relational DB vs NoSQL
  Relational DB provides nice ACID properties while NoSQL scales little better and has high availability
  Depending on the problem we need to pick the best

### 9. Types of NoSQL
  **Key value**
  
  **Wide column**
  
  **Document-based**
  
  **Graph-based**

### 10. Caching
  To speed up the request. Cache cannot be the source of truth. Cache has to be small because it stores data in-memory.
  Caching on every node
  Distributed cache - shared between nodes
  
  More on cache eviction policy

### 11. Data center / Racks / Hosts
  Data Centers have Racks which in turn have Hosts. We need to understand how these work, what is the latency between multiple racks / hosts. What happens when a host or a rack or a DC goes down?

### 12. CPU / Memory/ Hard drives / Network bandwidth
  We must be aware of the limitations and correspondingly improve throughput latencies and improve the system around these limited resources

### 13. Random vs Sequential read/writes to disk
  Sequential reads/writes are better for the disks

### 14. HTTP vs http2 vs WebSocket
  HTTP - Request-Response kind of architecture between client/structure
  HTTP2 - Improvements on the deficiencies of HTTP like multiple requests over single connection (Streams)
  WebSocket - Fully bi-directional communication between client & server.

### 15. TCP/IP model

### 16. ipv4 vs ipv6

### 17. TCP vs UDP

### 18. DNS lookup

### 19. Http & TLS

### 20. Public key infrastructure and Certificate Authority(CA)

### 21. Symmetric vs Asymmetric Encryption

### 22. Load Balancer

### 23. CDNs & Edges

### 24. Bloom filters and Count-Min sketch

### 25. Paxos 

### 26. Leader election

### 27. Design patterns and Object-Oriented Design

### 28. Virtual machines and containers

### 29. Pub-sub architecture 

### 30. MapReduce

### 31. Multithreading, locks, synchronization, CAS (compare and set)


# Tools

1. Cassandra
2. MongoDB/Couchbase
3. Mysql
4. Memcached / Redis (http://blog.andolasoft.com/2014/02/memcached-vs-redis-which-one-to-pick-for-large-web-app.html)
5. Zookeeper
6. Kafka
7. NGINX
8. HAProxy
9. Solr, Elastic search
10. Amazon S3
11. Docker, Kubernetes, Mesos
12. Hadoop/Spark and HDFS
