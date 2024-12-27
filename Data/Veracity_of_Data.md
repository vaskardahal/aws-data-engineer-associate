# Veracity of Data

* When there is data that is <ins>ungoverned</ins>, coming from numerous, dissimilar sources and this data <ins>cannot be curated</ins> in meaningful ways, there is a veracity problem. 
* Data changes over time. As it is transferred from one process to another, and through one system to another, there are opportunities for the integrity of the data to be negatively impacted.
* Bad data costs businesses money, time, and customers. 
* Not only is it a huge hassle to recover and fix mistakes, but it also reflects poorly on business as bad customer service in the process. 

### Definitions
* Curation
	* Curation is the action or process of selecting, organizing and looking after the items in a collection. 
* Data integrity
	* Data integrity is the maintenance and assurance of the accuracy, completeness and consistency of data over its entire life cycle. 
* Referential integrity
	* Referential integrity is the process of ensuring that the constraints of table relationships are enforced. 
* Domain integrity
	* Domain integrity is the process of ensuring that the data being entered into a field matches the data type defined for that field. 
* Entity integrity
	* Entity integrity is the process of ensuring that the values stored within a field match the constraints defined for that field. 
* Data veracity
	* Data veracity is the degree to which data is accurate, precise and trusted. 
	* Data veracity is contingent on the integrity of the data. 
* Data corruption
	* Data corruption refers to any unwanted change that happens to a file during storage, transmission or processing. 
	* A corrupted file\data can become unusable, inaccurate, unreadable or in some way inaccessible to a user or a related app. 
* Data cleansing
	* Data cleansing is the process of detecting and correcting corruptions within data. 
	* Data cleansing is applied as a part of ETL process. 
* Data schema
	* A data schema is the set of metadata used by the database to organize data objects and enforce integrity constraints - it is the main line of defense for maintaining data integrity. 
	* The schema defines the attributes of the database, providing descriptions of each object and how it interacts with other objects within the database. 
	* One or more schema can reside in the same database. 
* Information schema
	* An information schema is a database of metadata that houses information on the data data objects within a database. 
	* It also contains statistics on the distribution of data within tables, indexing and partitioning of the data. 

### Data Life cycle and Data integrity 

![Data Lifecycle](data_lifecycle.png)


## How to clean data? 
1. Know and define what clean data looks like. 
2. Identify the source of errors in the data. 
3. Build a consensus on what acceptable changes to the data looks like. 
	- Example: The average of a column differs when 0 is entered in the cells and these cells are left empty. So, should an empty cell be replaced by 0 or not? 
4. Identify if the original data (before transformation) value still exists or not and how\what it was. 


![How to preserve data integrity?](data_integrity_preservation.png)

