# Choosing the right NoSQL database for the job: a quality attribute evaluation

## Citation

```
Lourenço, J.R., Cabral, B., Carreiro, P., Vieira, M. and Bernardino, J., 2015. Choosing the right NoSQL database for the job: a quality attribute evaluation. Journal of Big Data, 2(1), pp.1-26.
```

## Contributions

* Develops a quality-attribute oriented evaluation of NoSQL databases.

  **Table 1.** *Summary table with characteristics of the selected NoSQL databases.*

  |                         | Aerospike                                                    | Cassandra                      | Couchbase                                                    | CouchDB                                                      | HBase                                          | MongoDB                                        | Voldemort                              |
  | ----------------------- | ------------------------------------------------------------ | ------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------------- | ---------------------------------------------- | -------------------------------------- |
  | **Category**            | Key Value                                                    | Column Store                   | Document Store                                               | Document Store                                               | Column Store                                   | Document Store                                 | Key Value                              |
  | **CAP**                 | AP                                                           | AP/CP                          | CP                                                           | AP                                                           | CP                                             | CP                                             | AP                                     |
  | **Consistency**         | Configurable (several options)                               | Configurable (several options) | Eventual Consistency                                         | Eventual Consistency                                         | Configurable (strong and eventual consistency) | Configurable (several options)                 | Read-Repair (client handles conflicts) |
  | **Durability**          | Notified written to replica nodes                            | Configurable (several options) | Configurable (several options)                               | Configurable (notified written to at least one disk)         | Configurable (several options)                 | Configurable (several options)                 | Notified written to desired nodes      |
  | **Querying**            | Internal API                                                 | Internal API, SQL like (CQL)   | Internal API (MapReduce)                                     | Internal API (MapReduce)                                     | Internal API                                   | Internal API, MapReduce, complex query support | Internal API (get, put, delete)        |
  | **Concurrency Control** | Read-committed isolation level (support for optimistic concurrency control) | MVCC                           | MVCC (application can select Optimistic or Pessimistic locking) | MVCC (application can select Optimistic or Pessimistic locking) | Optimistic locking with MVCC                   | Master-slave with multi-granularity locking    | Optimistic locking with MVCC           |
  | **Partitioning Scheme** | Proprietary (Paxos based)                                    | Consistent Hashing             | Consistent Hashing                                           | Consistent Hashing (third party)                             | Range Based                                    | Consistent Hashing                             | Consistent Hashing                     |
  | **Native Partitioning** | Yes                                                          | Yes                            | Yes                                                          | No                                                           | Yes                                            | Yes                                            | Yes                                    |

  **Table 2.** *Summary table of different quality attributes studied for the selected NoSQL databases.*

  |                        | Aerospike | Cassandra | Couchbase | CouchDB  | HBase    | MongoDB  | Voldemort |
  | ---------------------- | --------- | --------- | --------- | -------- | -------- | -------- | --------- |
  | **Availability**       | Great     | Great     | Great     | Great    | Mediocre | Mediocre | Great     |
  | **Consistency**        | Great     | Great     | Good      | Good     | Average  | Great    | Good      |
  | **Durability**         | Mediocre  | Good      | Good      | Mediocre | Good     | Good     | Good      |
  | **Maintainability**    | Good      | Average   | Good      | Good     | Mediocre | Average  | Mediocre  |
  | **Read-Performance**   | Good      | Mediocre  | Great     | Average  | Mediocre | Great    | Good      |
  | **Recovery Time**      | Great     | Bad       | Good      | Unknown  | Unknown  | Great    | Unknown   |
  | **Reliability**        | Mediocre  | Good      | Mediocre  | Good     | Good     | Great    | Unknown   |
  | **Robustness**         | Good      | Good      | Average   | Average  | Bad      | Average  | Unknown   |
  | **Scalability**        | Great     | Great     | Great     | Mediocre | Great    | Mediocre | Good      |
  | **Stabilization Time** | Bad       | Good      | Good      | Unknown  | Unknown  | Bad      | Unknown   |
  | **Write-Performance**  | Good      | Great     | Good      | Mediocre | Good     | Mediocre | Great     |

* Creates a survey of the literature on the evaluation of NoSQL databases from a historic perspective.
  
  * There are ***4 clearly distinct periods*** of the evolution of NoSQL research:
    * ***Database type characterization*** (where NoSQL was in its infancy and researcher tried to categorize databases into different groups).
    * ***Performance evaluations***, with the advent of YCSB and a surge in NoSQL popularity.
    * ***Real-world scenarios*** and criticism to some ***interpretations of the CAP theorem***.
    * An even bigger focus on ***applicability*** and a reinvigorated focus on ***the validation of benchmarking software***.
  * There is not enough information to verify how suited each NoSQL database is in a specific scenario or system.
  * Each working system differs from another and all the necessary functionality and mechanisms highly affect the database choice.
  
* Identifies several future research directions towards the full coverage of software quality attributes in the evaluation of NoSQL databases.
  * There is a current need for a broad study of quality attributes in order to better understand the NoSQL ecosystem.
  * Research is currently ***lacking in terms of Reliability, Robustness, Durability and Maintainability***, with most work in literature focusing on raw performance.
  * The development of a framework for assessing most of these quality attributes would be greatly beneficial.