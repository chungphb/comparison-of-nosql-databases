# Consistency models of NoSQL databases

## Citation

```
Diogo, M., Cabral, B. and Bernardino, J., 2019. Consistency models of NoSQL databases. Future Internet, 11(2), p.43.
```

## Contributions

Compares the consistency models provided by five of the most popular non-cloud NoSQL database systems: Redis, Cassandra, MongoDB, Neo4j, and OrientDB.

* Summary

  **Table 1.** *Consistency models comparison.*

  |               | Strong Consistency | Casual Consistency | Session Consistency | Eventual Consistency | Weak Consistency |
  | :-----------: | :----------------: | :----------------: | :-----------------: | :------------------: | :--------------: |
  |   **Redis**   |                    |                    |                     |          x           |                  |
  | **Cassandra** |         x          |                    |                     |          x           |                  |
  |  **MongoDB**  |         x          |         x          |          x          |          x           |                  |
  |   **Neo4j**   |         x          |         x          |                     |          x           |                  |
  | **OrientDB**  |         x          |                    |          x          |          x           |                  |

  **Table 2.** *Consistency, Availability, and Network Partition Tolerance (CAP) Theorem and classification of databases based on their default configurations.*

  | CAP  | Databases              |
  | :--- | :--------------------- |
  | AC   | Neo4j, OrientDB, RDBMS |
  | CP   | MongoDB, Redis         |
  | AP   | Cassandra              |

* Conclusions
  * To be partition tolerant and ensure high consistency, uses MongoDB.
  * To provide high availability, uses Cassandra.
  * To offer high consistency whenever partition intolerance or non-distributed databases are an option, uses Neo4j or OrientDB.