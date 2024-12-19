# Velocity of Data

* When businesses need rapid insights from the data they are collecting, but the systems in place simply cannot meet that need, there is a velocity problem. 
* The speed at which the data is being generated is ever-accelerating. This data must be collected, processed, stored and analyzed at high speed.
* We require text messages to be sent and delivered instantly, but we can wait a few minutes for an email. These represent different velocity expectations. 
* The collection and processing of data have been combined into a single concept called data processing. 
* **Data Processing** means the collection and manipulation of data to produce meaningful information. 
* Between collecting and processing data, it is data processing where most of the time will be spent. 

![Processing Data](processing_data.png)


### Batch Processing
* Types:
	* Scheduled
	* Periodic
* Provides deep insights from complex analytics. 
* Example: Monthly credit card statements. 


### Stream Processing
* Types:
	* Near Real-time
	* Real-time
* Provides initial insights and real-time feedback. 
* Example: Text message moments after swapping credit card. This is a streaming data for fraud prevention alert and happens instantaneously. 


### Comparison of Batch and Stream Processing

|             | Batch Processing                                                  | Stream Processing                                                           |
| ----------- | ----------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Scope       | Queries or processing over all or most of the data in the dataset | Queries or processing over data within a rolling time window                |
| Size        | Large batches\bursts of data                                      | Individual records or micro batches\bursts consisting only of a few records |
| Performance | Latencies in minutes to hours                                     | Requires latency in the order of seconds or milliseconds                    |
| Analysis    | Complex analytics                                                 | Simple response functions, aggregates, and rolling metrics                  |
