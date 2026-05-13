# DP-203 Glossary

| Term | Definition |
| --- | --- |
| **ADLS Gen2** | Azure Data Lake Storage Gen2 - hierarchical namespace over Blob. |
| **Parquet** | Columnar file format - default for analytics. |
| **Delta Lake** | Parquet + transaction log = ACID, upsert, time travel. |
| **Avro** | Row-based schema-aware format - good for streaming. |
| **Synapse Analytics** | Unified workspace: SQL pools + Spark + pipelines. |
| **Dedicated SQL pool** | MPP T-SQL data warehouse. |
| **Serverless SQL pool** | Pay-per-query SQL over the lake. |
| **Mapping Data Flows** | Visual GUI ETL in ADF/Synapse (Spark engine). |
| **Integration Runtime** | ADF compute - Azure / Self-hosted / SSIS. |
| **Hash distribution** | Synapse SQL data placement on a key. |
| **Round-robin distribution** | Even row distribution, no co-location. |
| **Replicate distribution** | Copy small table to each compute node. |
| **Star schema** | Fact + dimensions data model. |
| **SCD Type 1** | Overwrite on change. |
| **SCD Type 2** | New row per change with effective dates. |
| **Stream Analytics** | Azure SQL-like real-time streaming. |
| **Structured Streaming** | Spark streaming DataFrames API. |
| **Tumbling window** | Fixed non-overlapping interval. |
| **Hopping window** | Fixed window with hop period. |
| **Sliding window** | Continuous slide; outputs on each event. |
| **Session window** | Activity grouped by gaps. |
| **Event time** | Timestamp from event source. |
| **TDE** | Transparent Data Encryption. |
| **CMK** | Customer-Managed Key (via Key Vault). |
| **DDM** | Dynamic Data Masking. |
| **RLS** | Row-Level Security. |
| **CLS** | Column-Level Security. |
| **Purview** | Data catalog + classification + lineage. |
| **KQL** | Kusto Query Language. |
