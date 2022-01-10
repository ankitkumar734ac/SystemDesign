### Interview Questions
 

Q 1. Where does Scaling is required?
Backend apps, Webapps, DB Designs, App Servers, Caching Instances.

Q 2. How do we build Scalable Systems?  (AWS)
1. Designing DB according to requirements. If partitioning needs to be done at a later stage, we can easily break tables.
2. Write less complex and simple code, easy to deploy.
3. Write performant, efficient code to scale the system at any stage.

Q 3. Difference between Latency and ThroughPut.  (Microsoft) 
Latency- The total time taken by the system to complete an action and return a response. 
Throughput-  Throughput is the total number of actions performed in a unit of time. 

Q 4.  What is the relationship between throughput and latency with respect to System design? (Atlassian)
An ideal system is designed to provide maximum throughput and less latency.

Q 5. What is the difference between Weak, Strong, and Eventual Consistency? (Facebook)
Consistency depends on reading and writes operations on Database for any request.
Weak Consistency is may or may not be reading data without checking the latest write operation.
Eventual Consistency-  Reading data is eventually checking write operation. 
Strong Consistency- Reading data needs to be done after checking the write operation. 

Q 6. What are availability patterns?  (Gojek)
FailOver-  In failover, servers are either active or passive. If the active server fails, then the passive server starts serving the request. In the case of both active servers, requests are served by both. 
Replication- Master-Slave architecture of Database design, we replicate master DB and perform a read-write operation from master-slave, and in case the master is down, we can use slave DB,
