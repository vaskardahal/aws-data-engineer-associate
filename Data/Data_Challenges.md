

## 5 Vs of Big Data

1. Volume
2. Velocity
3. Variety
4. Veracity
5. Value


### Volume
* Amount of Data the solution must handle
* Solution must be able to do it efficiently, and must be able to distribute the load across servers to handle the velocity

### Velocity
* Speed at which data enters and flows through processes in the solution
* Since lot of organizations produce and deal with a large volume of real-time streaming data at a high frequency, a solution must be able to ingest and process all this data rapidly and without any lag

### Variety
* Solution should be able to ingest data of many different types from many different sources

### Veracity
* Trustworthiness of the data
* Chain of custody of data - ensuring that the data has not been altered falsely
* Collecting data can be easy, ensuring that the data is accurate and consistent is more challenging

### Value
* Deriving meaning and actionable insights from the data, by creating reports and dashboards
* Data should allow to make critical business decisions


## Throughput vs Latency

### Throughput
* Throughput refers to the rate at which data can be transmitted in unit time
* It determines how quickly data can be ingested, processed, and stored
* It is essential for scenarios where large amounts of data need to be ingested continuously

Latency
* Latency refers to the time delay between the initiation of an action and the occurrence of its effect
* Low latency is critical for real-time applications
* High latency can impact the responsiveness of applications and delay critical insights derived from ingested data


## Replaybility - Stateful\Stateless Transactions

### Stateful Applications
* Retain the state or memory of past interactions and data itself
* State information is remembered and stored by the application often on a server or in a database
* They might also maintain a memory of previous client interactions, allowing them to remember context and past actions
* Client sessions in a web application, online games that track user progress

### Stateless Applications
* Do not retain session data or memory of past transactions
* Each new request is processed individually without the knowledge of previous request
* Client state information is also not stored in the application server - so a client is required to send all the necessary information with each request
* Request-Response model is common in designing solution


### Replaybility
* Refers to the ability of a data ingestion system to reprocess or re-ingest the data that has already been processed, from a specific point in time
* Involves the ability to rerun or replay the data pipelines, workflows or ingestion processes to ensure data integrity, consistency, correctness or to address errors that might have occurred during initial ingestion
* Important for data recovery, backfilling historical data, testing and debugging
* Usage: 
	* Error handling
	* Data consistency : consistency in data needs to be maintained across distributed systems, and that might entail reprocessing the data
	* Upstream changes: When the data schema and format changes upstream (data source), it might become necessary to re-ingest the data 
	* Testing, development and debugging: Re-ingest the same data again and again to simulate scenarios without affecting the live data
* Implementation strategies: 
	* Idempotent Operations: Designing processes to be idempotent in the source so that replaying the same data does not result in duplicate records or unintended side-effects.
	* Logging and Auditing
	* Checkpointing: Implementing checkpoints or markers at various stages of ingestion pipeline. It helps identify the point from which the data needs to be replayed.
	* Backfilling: Backfilling data from a specific timestamp or event, without reprocessing entire data
* Challenges of Replaybility:
	* Idempotency: Replaying the data does not cause duplicate records, which is a challenge in distributed systems or when complex data transformations need to be carried out. 
		* Order Dependency
		* Data Dependency
	* Data volume and performance: Reingesting large volume of data can strain the system and impact performance. This may also result in latency - especially when timeliness of the data availability is crucial. 
	* Resource management: Storage, network bandwidth, cost considerations
	* Consistency: Challenging to ensure consistency in replayed data, ensuring that new errors are not introduced
	* Data Retention Policies

## Data Volume Challenges
- The International Data Corporation (IDC) forcasts massive growth in data between now and 2050. the corporation predicts that the Global Datasphere - which is all the data that's collected, everywhere - will grow from 33 zettabytes in 2023 to 175 zettabytes by 2050. 
- A data analysis solution has to support large, scalable and durable data storage. It must also be able to gather data from multiple sources. 



## Six Layers of Modern Data Architecture
#### 1. Data Ingestion
* Bring the data into the central data platform, like AWS.

#### 2. Data Storage
* Store structured and unstructured data. 

#### 3. Data Cataloging
* Develop and store metadata for the data. 

#### 4. Data Processing
* Create data processing pipelines.

#### 5. Data Consumption
* Enable user personas for purpose-built analytics & machine learning.

#### 6. Data Governance
* Protect data across the layers and data access management. 

