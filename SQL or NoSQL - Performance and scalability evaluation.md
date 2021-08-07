# SQL or NoSQL? Performance and scalability evaluation

## Citation

```
Abramova, V., Bernardino, J. and Furtado, P., 2015. SQL or NoSQL? Performance and scalability evaluation. International Journal of Business Process Integration and Management, 7(4), pp.314-321.
```

## Contributions

* Evaluates the scalability and the capability of NoSQL databases, represented by Cassandra, using Yahoo! Cloud Serving Benchmark (YCSB).
  * Cassandra is highly scalable and provides good horizontal scalability.
  * Cassandra is fast for execution of CRUD operations and key value access.
  * However, Cassandra lags behind in the capacity to execute decision support queries.
* Compare Hadoop and MySQL for execution of real enterprise queries using Star Schema Benchmark.
  * MySQL shows better results than Hadoop.
  * There are queries that could not run on Hadoop.
  * Because NoSQL fell short during execution of complex queries, they are not suited for decision support systems.

