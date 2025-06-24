# billing-records
serverless architecture in Azure
services stores billing records in Azure Cosmos DB. The system is read-heavy, but records older than three months are rarely accessed.
database size has significantly grown, leading to increased costs, need an efficient way to reduce costs while maintaining data availability.
Each billing record can be as large as 300 KB.
The database currently holds over 2 million records.
When an old record is requested, still be served, with a response time in the order of seconds.
