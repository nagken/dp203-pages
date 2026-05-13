# DP-203 Exam Cheatsheet

Quick-reference highlights. Skim before the exam.

- Lake = raw/curated zones (ADLS Gen2). Warehouse = star schema (dedicated SQL pool / Fabric).
- Parquet for analytics (columnar). Delta for ACID + upserts. Avro for streaming (row).
- Distribution: Hash large facts, Round-robin staging, Replicate small dims (<2GB).
- Partition by date/region; avoid low-cardinality + small files.
- SCDs: Type 1 overwrite, Type 2 history (new row), Type 6 hybrid.
- Serverless SQL: pay-per-query over lake; dedicated SQL: MPP warehouse; Spark: code/big data.
- ADF / Synapse Pipelines orchestrate. Mapping Data Flows = visual Spark ETL.
- Stream Analytics windows: tumbling (fixed), hopping (overlap), sliding (continuous), session (gap), snapshot (same ts).
- Event time > processing time for analytics correctness; use watermarks for late events.
- Integration Runtime: Azure / Self-hosted / Azure-SSIS.
- Triggers: schedule / tumbling / event / manual.
- TDE = default at-rest enc. CMK for customer-controlled keys via Key Vault.
- RLS = rows (predicate). CLS = columns (grant). DDM = display masking (not security).
- Managed Identity > Service Principal > SAS > Account Key (worst).
- Purview = catalog + classification + lineage.
- Monitor: Azure Monitor + Log Analytics (KQL) + Synapse Monitor + Query Store / Spark UI.
- Compact small files; UPDATE STATISTICS after bulk loads; partition prune.
