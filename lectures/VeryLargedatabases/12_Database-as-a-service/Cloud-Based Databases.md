Database systems hosted and managed in the cloud, rather than on local or on-premise infrastructure.
- Initial cloud [[Database Management Systems (DBMS)]] offerings repackaged [[On-Premise Systems]] into managed VMs with [[Direct-Attached Storage (DAS)]] 
- All major cloud vendors offer [[Network-Attached Storage (NAS)]] via object stores (example: [[Amazon S3]]) with some [[Database Management Systems (DBMS)]] functionality (example: [[Replication]], [[Filtering]])
- Compute nodes are disconnected from the storage nodes, a system can provide [[Per-Query Elasticity]]; the [[Database Management Systems (DBMS)]] can add new compute nodes dynamically without having reshuffle data
- "Pushing the query to the data" vs "Pulling the data to the query". Both possible
- "[[Serverless Computing]]" was introduced for cloud-native [[Database Management Systems (DBMS)]] by [[Snowflakes]]
- Hosted multi-node environment in which multiple [[Database Management Systems (DBMS)]] customers are grouped onto the same node(s) with a [[Multi-Tenancy]] execution scheme
- Has impacted [[Database Management Systems (DBMS)]], causing them to be completely re-architected
- Vendors can track usage trends for all their customers: They can monitor unexpected behaviour, [[Performance]] degradations and usage patterns
- Open-Source [[Database Management Systems (DBMS)]] face the danger of becoming too popular and being monetised by the major cloud providers. The public spats between Amazon and [[Independent Software Vendor (ISV)]] like [[MongoDB]] and [[ElasticSearch]]