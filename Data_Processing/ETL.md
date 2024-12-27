# Extract, Transform and Load

* ETL is the process of collecting data from raw data sources and then transforming the data into common types and formats. This data is then loaded into final destination to become available for analytical applications and inspection. 
* ETL is all about transforming data so that we can build purpose-built datasets - which can be used to develop advanced analytical results.
* Transformed data can dramatically reduce the time and cost of overall analysis. 
* Extract: 
	* Need to know where the source data resides and how to access them. 
	* Needs to take into consideration the potential impacts of read and copy steps on the source system. 
	* Initial and consecutive data extraction must also be planned - like the frequency of extraction. 
	* Also, need to plan where to store the data during the extract operation. This is called the staging location. 
* Transformation: 
	* Transformation can be very basic - like cleaning data, data formatting, replacing data values (like replacing NULL values). 
	* And it can be very advanced like applying business rules to the data to calculate new values. Advanced transformation include filtering record, complex join operations, aggregating rows, splitting columns and data validation. 
	* It can also be combining of two different datasets to get insights. 
	* It can also be used to perform data cleansing - like reconciling between CA and California in address. 
	* Denormalization: Data normalized for databases loses its significance for analytical usage. Analytical systems require data to be organized so that the queries can be simplified and quickly generated to produce aggregates. 
	* Changing data storage types: Transforming NoSQL data to relational data and vice versa. 
	* Destination compatibility: Ensuring that the data is in the format acceptable to the intermediate or final load destination. 
* Load: 
	* 

![ETL](etl.png)

![ETL II](etl_II.png)

![Transformation to combine two datasets](combining_two_datasets.png)

![Loading Data](loading_data.png)


## AWS Glue vs Amazon EMR

| Parameters                | AWS Glue             | Amazon EMR           |
| ------------------------- | -------------------- | -------------------- |
| Deployment Types          | Serverless           | Server Platform      |
| Pricing                   | High                 | Low                  |
| Flexibility & Scalability | Flexible             | Harder to scale      |
| Primary Purpose           | ETL operations       | Big data processing  |
| Performance               | Slow and less stable | Fast and more stable |

