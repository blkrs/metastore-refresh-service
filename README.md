# metastore-refresh-service
Service for refreshing metastore data about tables for Impala

## REST endpoints

Table names can contain database prefix. So **default.table** is accepted by the service

* **/** returns status message
* **/refres/<table>** refreshes single table
* **/invalidate/** invalidates whole metastore
* **/invalidate/<table>** invalidates data related to only one table

