# NoSQL Databases

* NoSQL databases (aka "not only SQL") are non-tabular databases and store data differently than relational tables. 
* They provide flexible schemas and scale easily with large amounts of data and high user loads. 
* NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column and graph. 
* Data redundancy is common in NoSQL database, as opposed to relational databases which are normalized to minimize data redundancy. 
* Usage example of e-commerce site: A customer initiates a shopping cart in Amazon website, but decides to check out on a later date. That data in the shopping cart has to be dealt with. If the shopping cart data was stored in a relational database, there might be multiple records spanning across multiple tables. If the customer later on decides to abandon this cart, all these tables would have to be touched. But with NoSQL database, the entire shopping cart could be stored in a single record. If the customer checks out the shopping cart, then the data from the NoSQL record can be passed on to a relational database for permanent storage. The NoSQL record can then be deleted automatically. 

### Document store databases
* Document stores are a type of non-relational database that store semi-structured and un-structured data in the form of files. 
* These files range in form but include JSON, BSON and XML. 
* These files can be navigated using various scripting languages like Python and data processing tools like Glue+Athena. 
* Strengths: 
	* Flexibility: No need to plan for specific type of data when creating one. 
	* Scalibility: Easy to scale vertically. 
* Weaknesses: 
	* Sacrifice ACID compliance for flexibility. 
	* Cannot query across files without some additional aggregations or transformations. 

### Key-value databases
* Key-value databases are a type of non-relational database that store semi-structured data in the form of key-value pairs.
* Logically, data is stored in a single table. This table contains items, and each item contains one or more attributes. Each attribute is a key-value pair and serves as the functional unit. 
* The table in key-value database differs from that in relational database in that the table in key-value database is schema-less.
	* It also offers the advantage of creating nested attributes. A relational database would likely move such nested relationship into a different table. 
* Strengths:
	* Very flexible. 
	* Able to handle wide variety of data types. 
	* Keys are linked directly to their values with no need for indexing or complex join operations. 
	* Content of a key can easily be copied to other systems without reprogramming the data. 
* Weaknesses: 
	* Impossible to query values because they are stored as a single blob. 
	* Updating or editing the content of a value is quite difficult. 
	* Not all objects can be modeled as key-value pairs. 

### Graph databases
* Graph databases are about connections and relationships. 
* They are purpose-built to store any type of data - structured, semi-structured or unstructured. 
* The purpose of organization within a graph database is to navigate relationships. 
* Strengths: 
	* Allow simple, fast retrieval of complex hierarchical structures. 
	* Great for real-time big data mining. 
	* Can rapidly identify common data points between nodes. 
	* Great for making relevant recommendations and allows for rapid querying of those relationships. 
* Weaknesses: 
	* Cannot adequately store transactional data. 
	* Analysts must learn new languages to query the data. 
	* Performing  analytics on the data may not be as efficient as with other database types. 
* AWS service for graph database is called Amazon Neptune. 
* ![Amazon Neptune](amazon_neptune.png)
* Use cases: 
	* Social networking
	* Recommendation systems
	* Fraud detection


## Comparison

| Characterstic  | Relational Database                                  | Non-relational                                              | Graph                                  |
| -------------- | ---------------------------------------------------- | ----------------------------------------------------------- | -------------------------------------- |
| Representation | Multiple tables, each containing columns and rows.   | Collection of documents. Single table with keys and values. | Collection of nodes and relationships. |
| Data design    | Normalized relational or dimensional data warehouse. | Denormalized document, wide column or key value.            | Denormalized entity relationship.      |
| Optimized      | Optimized for storage.                               | Optimized for compute.                                      | Optimized for relationships.           |
| Query style    | Language: SQL                                        | Language: many. Uses object querying.                       | Language: many. Uses object querying.  |
| Scaling        | Scale vertically                                     | Scale horizontally                                          | Hybrid                                 |
| Implementation | OLTP business systems, OLAP data warehouse           | OLTP web/mobile apps                                        | OLTP web/mobile apps                   |