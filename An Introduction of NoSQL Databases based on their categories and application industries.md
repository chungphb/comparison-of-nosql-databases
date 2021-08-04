# An Introduction of NoSQL Databases based on their categories and application industries

## Citation

```
Chen, J.K. and Lee, W.Z., 2019. An Introduction of NoSQL Databases based on their categories and application industries. algorithms, 12(5), p.106.
```

## Contributions

* Introduces the basic characteristics of ***15 categories of NoSQL database***.

  | No.  | Category                          | Characteristics                                              | Example                                 |
  | :--: | --------------------------------- | ------------------------------------------------------------ | --------------------------------------- |
  |  1   | Wide Column Store                 | Three-dimensional data.<br />Applications that often search for specific field data. | Apache Cassandra, Apache HBase          |
  |  2   | Document Store                    | Semi-structured files, such as XML, JSON, and so on.         | MongoDB, Couchbase Server               |
  |  3   | Key Value Store                   | One-dimensional data, which is stored in key-value pairs.    | Redis, DynamoDB                         |
  |  4   | Graph Databases                   | Data stored in a graphic structure.<br />Suitable for data of social network relations, recommendation systems, and so on. | Neo4J, FlockDB                          |
  |  5   | Multimodel Databases              | Determine data features suitable processing based on the data format of a specific database. | OrientDB, ArangoDB                      |
  |  6   | Object Databases                  | The object-oriented concepts are used to describe the data itself and the relationship among the data.<br />Suitable for computer aided design (CAD) and office automation. | db4o, Versant                           |
  |  7   | Grid and Cloud Database Solutions | Applications that need to search recent access data frequently. | Hazelcast, Oracle                       |
  |  8   | XML Databases                     | Data stored in XML files.                                    | Oracle Berkeley DB, BaseX               |
  |  9   | Multidimentional Databases        | Applications that often analyze data in multiple dimensions. | intersystems cache, GT.M                |
  |  10  | Multivalue Databases              | Data with multivalued attributes or composite attributes.    | jBASE, Model 204 Database               |
  |  11  | Event Sourcing                    | Data with events that occurred in the past for tracking the status of something. |                                         |
  |  12  | Time Series Databases             | Data related to time series.                                 | InfluxDB, Informix Time Series Solution |
  |  13  | Other NoSQL Related Databases     | Unable to know.                                              | eXtremeDB                               |
  |  14  | Scientific and Specialized DBs    | Data suitable for scientific research or computing.          | BayesDB, GPUdb                          |
  |  15  | Unresolved and Uncategorized      | Data based on the data format of a specific database.        |                                         |

* Analyzes ***the characteristics of the data that each category of NoSQL database is suitable*** for processing.
* Proposes some ***principles and key points*** for reference to help enterprises ***to find an appropriate NoSQL database***.
  * Understands the current problems, goals, and challenges of the corporate operation database.
  * Decides to continue using the current RDB or change using a NoSQL database based on the needs of enterprise and their expertise.
  * If changing to use a NoSQL database, selects a suitable category of NoSQL databases based on the features and formats of corporate operating data.
  * When deciding which NoSQL database to choose, makes a decision according to the needs of the enterprise, the characteristics of each database, as well as the reputation and popularity of each database.
* Illustrates three cases (3C shopping website, newspapers, and the US retail industry) to demonstrate how to choose a suitable NoSQL database.

  * The transaction data of the e-commerce industry often needs to be related, so the suitable NoSQL DB category is the wide column store.
  * The news materials of the news industry have semi-structured features, so the suitable NoSQL DB category is the document store.
  * The retailer data needs to be used by the recommendation system, so the suitable NoSQL DB category is the graph databases.