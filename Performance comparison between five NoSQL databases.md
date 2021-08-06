# Performance comparison between five NoSQL databases

## Citation

```
Tang, E. and Fan, Y., 2016, November. Performance comparison between five NoSQL databases. In 2016 7th International Conference on Cloud Computing and Big Data (CCBD) (pp. 105-109). IEEE.
```

## Contributions

Compares the performance of 5 NoSQL databases (Redis, MongoDB, Couchbase, Cassandra, and HBase) through 2 experiments on a 4-node cluster.

* Summary
  * *Experiment 1:* Compares ***execution speed*** of the databases under certain conditions.
    * Data loading
      * Redis got the best performance.
      * Column-family databases, Cassandra and HBase, were slightly lower than Redis.
      * Couchbase presented the worst performance.
    * Workloads execution
      * Redis also got the best performance.
      * Column-family databases, Cassandra and HBase, were the slowest.
      * Document databases, MongoDB and Couchbase, presented good performance.
  * *Experiment 2:* Compares ***storage expansion tolerance*** of the databases.
    * Data loading
      * Redis was increasing at the fastest pace.
      * The throughput of Cassandra and Couchbase grew more rapidly compared to HBase and MongoDB.
    * Workloads execution
      * Redis still showed the best throughput performance.
      * Couchbase, Cassandra and HBase presented a similar trend as the loading stage (insertion process).
      * Throughput and efficiency of MongoDB decreased when the record exceeded a certain count limit.
* Conclusions
  * Redis is particularly well suited for loading and executing workloads but has its limitation when facing extremely large data.
  * Document databases, followed by column-family databases, have a good average performance.
  * ***Database framework in master-master mode***, where each node is equivalent, ***has more advantages over those in master-slave architectures***.
