# Experimental evaluation of NoSQL databases

## Citation

```
Abramova, V., Bernardino, J. and Furtado, P., 2014. Experimental evaluation of NoSQL databases. International Journal of Database Management Systems, 6(3), p.1.
```

## Contributions

Compares execution time of diverse requests for three types of NoSQL databases: Document Store, Column Family and Key-value Store, in order to better understand how performance of a database is affected by its type ***in a non-distributed environment***.

* Summary
  * Tarantool and Redis have the best result with extremely fast response times regardless of workloads.
  * Oracle NoSQL has the lowest performance on data loading.
  * OrientDB has the lowest performance on execution of a set of workloads.
  * HBase and Cassandra are especially optimized for performing updates, while reads are more time consuming when compared to in-memory databases.
  * MongoDB has the largest increase in execution time directly proportional to the number of performed updates.
  * According to the results, Tarantool is the database with the best performance.
* Conclusions
  * In terms of optimization, NoSQL databases can be divided into two categories, ***databases optimized for reads*** and ***databases optimized for updates***.
    * MongoDB, Redis, Scalaris, Tarantool and OrientDB are databases optimized to perform read operations.
    * Cassandra, Oracle NoSQL, HBase and Voldemort are databases optimized to perform update operations.