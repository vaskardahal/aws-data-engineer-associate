# Data Formats

### CSV

### JSON

### XML

### Avro

### Parquet


| AVRO                                                                                                                          | PARQUET                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Well-integrated with Apache Hadoop, Spark, Kafka                                                                              | Well-integrated with Apache Hadoop, Spark, Kafka                                  |
| Avro is supported by Apache impala                                                                                            | Parquet is optimized for Apache Impala                                            |
| Supports row-based storage                                                                                                    | Supports columnar storage                                                         |
| Uses a JSON-based schema to define the structure of the data                                                                  | Uses its own schema definition language                                           |
| Has separate files to store schema and data                                                                                   | Combines both schema and data into one file                                       |
| Used to achieve a compact binary format by allowing efficient serialization that results in smaller payloads compared to JSON | Used for applications that require data warehousing analytics (like aggregations) |

### Transforming data formats using Glue ETL jobs
#### 1. Python ETL jobs
* Suitable for simpler ETL tasks with small dataset. 
* Python Shell jobs in Glue offers prebuilt libraries for transforming data into other formats, for aggregating data and for reading data from files such as CSV, JSON and Parquet.
#### 2. Spark ETL jobs
* Suitable for workloads requiring high compute power. 
* Spark ETL jobs in Glue can perform complex data transformations over large-scale data. 
* Spark transformations include: filtering, aggregating, and joining data from multiple datasets. 
#### 3. Batch and Stream Processing jobs (using PySpark or Scala)
* PySpark or Scala can be used to write jobs that handle both:
	* Traditional batch processing: processing data in fixed-size batches. 
	* Streaming data processing: processing data in micro-batches at regular intervals. 

