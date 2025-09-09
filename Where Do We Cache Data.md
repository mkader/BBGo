There are multiple layers along the flow.
* Client apps: HTTP responses can be cached by the browser. We request data over HTTP for the first time, and it is returned with an expiry policy in the HTTP header; we request data again, and the client app tries to retrieve the data from the browser cache first.
* CDN: CDN caches static web resources. The clients can retrieve data from a CDN node nearby.
* Load Balancer: The load Balancer can cache resources as well.
* Messaging infra: Message brokers store messages on disk first, and then consumers retrieve them at their own pace. Depending on the retention policy, the data is cached in Kafka clusters for a period of time.
* Services: There are multiple layers of cache in a service. If the data is not cached in the CPU cache, the service will try to retrieve the data from memory. Sometimes the service has a second-level cache to store data on disk.
* Distributed Cache: Distributed cache like Redis hold key-value pairs for multiple services in memory. It provides much better read/write performance than the database.
* Full-text Search: we sometimes need to use full-text searches like Elastic Search for document search or log search. A copy of data is indexed in the search engine as well.
* Database: Even in the database, we have different levels of caches:
  * WAL(Write-ahead Log): data is written to WAL first before building the B tree index
  * Bufferpool: A memory area allocated to cache query results
  * Materialized View: Pre-compute query results and store them in the database tables for better query performance
  * Transaction log: record all the transactions and database updates
  * Replication Log: used to record the replication state in a database cluster
 
<img src="https://github.com/mkader/BBGo/blob/main/Where%20Do%20We%20Cache%20Data.jpg">
