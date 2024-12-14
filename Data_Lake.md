# Data Lake Architecture

![[modern_data_architecture.png]]

* A Data Lake is a centralized repository that allows to store all structured and unstructured data at any scale.
* Data lake can store data as-is, without having to first structure the data. 
* And it also allows to run different types of analytics - from dashboards and visualizations to big data processing, real-time analytics, and machine learning to guide better decisions. 
* No matter how data gets into S3, there should be a meaningful way to organize it and find it when required. And that is where Data Lake comes in. 
* Data lake is an architectural concept that helps to manage multiple data types from multiple sources through a single set of tools. 
* In other words, data lake takes Amazon S3 buckets and organizes them by categorizing them by data inside the buckets - irrespective of how the data got there or what kind of data it is. 
![[data_lake.png]]

### Why Data Lake? 
* Many organizations end up grouping data into numerous storage locations called silos.
* These silos are rarely managed and maintained by the same team, and that can be problematic. 
* Inconsistencies in the way the data was written, collected, aggregated or filtered can cause problems when it is compared or combined for processing from different silos. 
* For example, one team can use the Address field to store both the street number and street name, while the other team can use two different fields to store street name and street number. Thus, there is an inconsistency in the way data is stored. 
* But by using data lake, these silos can be broken down and data can be brought into single central repository that is managed by a single team and thus provide single consistent source of truth for the data. 
* Data lake in AWS is a solution that guarantees single repository of data storage in a generally less expensive and less specialized manner than big data storage solutions like Data Warehouse. 
### Benefits of Data Lake
* Store all data in open formats - no special format requirement. 
* Cost-effective way of storing data in a scalable fashion - can be scaled to exabytes. 
* Decouple storage from compute. 
* Choice of analytical and ML engines. 
* Process data in a single place. 



![[data_lake_architecture.png]]


![[modern_data_architecture_II.png]]