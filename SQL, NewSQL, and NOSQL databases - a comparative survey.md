# SQL, NewSQL, and NOSQL databases: a comparative survey

## Citation

```
Khasawneh, T.N., AL-Sahlee, M.H. and Safia, A.A., 2020, April. SQL, NewSQL, and NOSQL databases: a comparative survey. In 2020 11th International Conference on Information and Communication Systems (ICICS) (pp. 013-021). IEEE.
```

## Contributions

Provides an overview of DB technologies and acts as a resource of the different non-relational databases to help people choose the suitable technology for their specific application.

* The advantages and disadvantages of RDBMS, NewSQL, and NoSQL.

* An overview about the metrics commonly used to compare the different NoSQL models.

  * Persistence
  * Replication
  * Sharding
  * Consistency
  * Query method
  * Implementation language

* The comparison of different NoSQL databases.

  **Table 1.** Key-value databases and their characteristics

  |                | Persistence                                                  | Replication     | Sharding           | Consistency                  | API                            | Query method                         | Implementation language | CAP       |
  | -------------- | ------------------------------------------------------------ | --------------- | ------------------ | ---------------------------- | ------------------------------ | ------------------------------------ | ----------------------- | --------- |
  | **Riak**       | Bitcask, LevelDB, In Memory and Multi backend                | Ring (next N-1) | Consistent Hashing | Tunable (Eventual or Strong) | PBC                            | REST-ful API, Apache Solr, MapReduce | Erlang                  | AP        |
  | **Infinispan** | Simple File Storage, BerkeleyDB, JDBM, JDBC                  | Ring (next N-1) | Consistent Hashing | Tunable                      | HTTP, Java                     | Get, MapRedu ce                      | Java                    | AP/AC/C P |
  | **Hazelcast**  | User-defined MapStore                                        | Ring (next N-1) | Consistent Hashing | Strong                       | HTTP, Java, C#                 | Get, MapRedu ce                      | Java                    | AP        |
  | **Redis**      | Snapshots at specified intervals by default or an append-only file. Both can becombined. | Master-Slave    | Not supported      | Eventual                     | Java, C, C#, Ruby, Perl, Scala | Get                                  | C                       | AP        |
  | **Voldemort**  | BerkeleyDB, In Memory, MySQL                                 | Ring (next N-1) | Consistent Hashing | Eventual                     | Java, Python                   | Get                                  | Java                    | AP        |
  
  **Table 2.** Column-oriented databases and their characteristics
  
  |                | Persistence        | Replication                   | Sharding                           | Consistency | API                                   | Query method   | Implementation language | CAP  |
  | -------------- | ------------------ | ----------------------------- | ---------------------------------- | ----------- | ------------------------------------- | -------------- | ----------------------- | ---- |
  | **HBase**      | HDFS               | HDFS                          | By key value, allows auto sharding | High        | Java, REST-ful, Thrift, Avro          | MapReduce      | Java                    | CP   |
  | **Hypertable** | HDFS               | HDFS                          | By key value, allows chunking      | High        | C++ API, Java, REST-ful, Thrift, Avro | MapReduce, HQL | C++                     | CP   |
  | **Cassandra**  | Proprietary format | Auto partition with zero loss | By row                             | Eventual    | CQL, Thrift                           | MapReduce      | Java                    | AP   |
  | **Accumulo**   | HDFS               | Multi master replication      | By row                             | Eventual    | Java, REST-ful, Thrift                | MapReduce      | Java                    | CP   |
  
  **Table 3.** Document-oriented databases and their characteristics
  
  |                | Persistence                | Replication   | Sharding                  | Consistency        | API                                         | Query method                 | Implementation language | CAP   |
  | -------------- | -------------------------- | ------------- | ------------------------- | ------------------ | ------------------------------------------- | ---------------------------- | ----------------------- | ----- |
  | **CouchDB**    | B-Tree                     | Master-Master | Available with extensions | Eventual           | HTTP and JSON                               | MapReduce                    | Erlang                  | AP    |
  | **MongoDB**    | BSON objects, GRIDFS       | Master-Slave  | By field                  | Strict or Eventual | HTTP and JSON, Mongo wire protocol and BSON | By field, cursors, MapReduce | C++                     | AP/CP |
  | **Terrastore** | Terrastore storing support | Master-Slave  | By field                  | Eventual           | HTTP and JSON                               | Conditional queries          | Java                    | AP    |
  | **RavenDB**    | Extensible storage engine  | Master-Slave  | User defined              | Eventual           | HTTP and JSON, .NET                         | MapReduce, LINQ              | C#                      | AP    |
  
  **Table 4.** Graph databases and their characteristics
  
  |                   | Persistence                 | Replication  | Sharding   | Consistency | API                   | Query method                   | Implementation language | CAP   |
  | ----------------- | --------------------------- | ------------ | ---------- | ----------- | --------------------- | ------------------------------ | ----------------------- | ----- |
  | **Neo4J**         | Apache Lucene               | Master-Slave | Manual     | Eventual    | Java, HTTP and JSON   | Java API                       | Java                    | AP    |
  | **InfiniteGraph** | Objectivity                 | Peer to Peer | Rule-based | Tunable     | C++, Java, Python, C# | Graph traversal API            | C++                     | AP/CP |
  | **InfoGrid**      | MySQL, HDFS                 | Peer to Peer | Manual     | Eventual    | Java, HTTP and JSON   | Viewlets, Templates HTML, Java | Java                    | AP    |
  | **HypergraphDB**  | Relations caching + Indexes | Peer to Peer | Manual     | Eventual    | Java                  | Java API                       | Java                    | AP    |
  | **BigData**       | Indexes (B+ trees)          | Master-Slave | Dynamic    | Eventual    | Java                  | SPARKQL, RDFS++                | Java                    | AP    |
  | **AllegroGraph**  | Indexes                     | Master-Slave | Manual     | Eventual    | HTTP and JSON         | SPARQL, Graph traversal API    | Lisp                    | AP    |