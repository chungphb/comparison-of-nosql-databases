# NoSQL evaluation: A use case oriented survey

## Citation

```
Hecht, R. and Jablonski, S., 2011, December. NoSQL evaluation: A use case oriented survey. In 2011 International Conference on Cloud and Service Computing (pp. 336-341). IEEE.
```

## Contributions

Compares the advantages and disadvantages of 14 NoSQL databases in terms of ***query possibilities***, ***concurrency control***, ***partitioning***, ***replication*** and ***consistency***.

* Result

  **Table 1.** *Query possibilities*

  |                | REST API | JAVA API | Query Language | Map Reduce Support |
  | :------------- | :------: | :------: | :------------: | :----------------: |
  | **Voldemort**  |    -     |    +     |       -        |         -          |
  | **Redis**      |    -     |    +     |       -        |         -          |
  | **Membase**    |    +     |    +     |       -        |         -          |
  | **Riak**       |    +     |    +     |       -        |         +          |
  | **MongoDB**    |    +     |    +     |       -        |         +          |
  | **CouchDB**    |    +     |    +     |       -        |         +          |
  | **Cassandra**  |    -     |    +     |       +        |         +          |
  | **HBase**      |    +     |    +     |       +        |         +          |
  | **Hypertable** |    -     |    +     |       +        |         +          |
  | **Sesame**     |    +     |    +     |       +        |         -          |
  | **BigData**    |    +     |    +     |       +        |         -          |
  | **Neo4j**      |    +     |    +     |       +        |         -          |
  | **GraphDB**    |    +     |    +     |       +        |         -          |
  | **FlockDB**    |    -     |    +     |       -        |         -          |

  **Table 2.** *Concurrency control*

  |                | Locks | Optimistic Locking | MVCC |
  | :------------- | :---: | :----------------: | :--: |
  | **Voldemort**  |   -   |         +          |  -   |
  | **Redis**      |   -   |         +          |  -   |
  | **Membase**    |   -   |         +          |  -   |
  | **Riak**       |   -   |         -          |  +   |
  | **MongoDB**    |   -   |         -          |  -   |
  | **CouchDB**    |   -   |         -          |  +   |
  | **Cassandra**  |   -   |         -          |  -   |
  | **HBase**      |   +   |         -          |  -   |
  | **Hypertable** |   -   |         -          |  +   |
  | **Sesame**     |   +   |         -          |  -   |
  | **BigData**    |   -   |         -          |  -   |
  | **Neo4j**      |   +   |         -          |  -   |
  | **GraphDB**    |   -   |         -          |  +   |
  | **FlockDB**    |   -   |         -          |  -   |

  **Table 3.** *Partitioning*

  |                | Range-based Hashing | Consistent Hashing |
  | :------------- | :-----------------: | :----------------: |
  | **Voldemort**  |          -          |         +          |
  | **Redis**      |          -          |         +          |
  | **Membase**    |          -          |         +          |
  | **Riak**       |          -          |         +          |
  | **MongoDB**    |          +          |         -          |
  | **CouchDB**    |          -          |         +          |
  | **Cassandra**  |          -          |         +          |
  | **HBase**      |          +          |         -          |
  | **Hypertable** |          +          |         -          |
  | **Sesame**     |          -          |         -          |
  | **BigData**    |          -          |         +          |
  | **Neo4j**      |          -          |         -          |
  | **GraphDB**    |          -          |         -          |
  | **FlockDB**    |          -          |         +          |

  **Table 4.** *Replication and Consistency*

  |                | Read from Replica | Write to Replica | Consistency |
  | :------------- | :---------------: | :--------------: | :---------: |
  | **Voldemort**  |         +         |        -         |     +/-     |
  | **Redis**      |         +         |        -         |      -      |
  | **Membase**    |         -         |        -         |      +      |
  | **Riak**       |         +         |        -         |     +/-     |
  | **MongoDB**    |         +         |        -         |     +/-     |
  | **CouchDB**    |         +         |        +         |      -      |
  | **Cassandra**  |         +         |        -         |     +/-     |
  | **HBase**      |         -         |        -         |      +      |
  | **Hypertable** |         -         |        -         |      +      |
  | **Sesame**     |         -         |        -         |      +      |
  | **BigData**    |         +         |        -         |      +      |
  | **Neo4j**      |         +         |        +         |      -      |
  | **GraphDB**    |         -         |        -         |      +      |
  | **FlockDB**    |         +         |        +         |     +/-     |

* Conclusions

  * Key value stores should be used for very fast and simple operations.
  * Document stores should be used for flexible data model with great query possibilities.
  * Column family stores should be used for very large datasets which have to be scaled at large size.
  * Graph databases should be used in domains, where entities are as important as the relationships
    between them.
