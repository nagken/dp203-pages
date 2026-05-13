# Extra DP-203 concepts

Deeper-dive concepts beyond the basics.

## Lambda vs Kappa architecture

Lambda = batch + speed layers reconciled. Kappa = streaming-only path. Most modern Azure designs prefer Kappa with replay (Event Hubs Capture).

## Medallion architecture

Bronze (raw) -> Silver (cleaned/conformed) -> Gold (curated/analytics-ready) zones.

## Polybase / OPENROWSET

External tables to query lake files directly from SQL.

## CTAS (Create Table As Select)

Primary load pattern in dedicated SQL pool (parallel + minimal logging).

## Caching: Result-set cache

Synapse caches query results for repeated identical queries.

## Workload management

Resource classes / workload groups in dedicated SQL pool to prioritize jobs.

## DP-203 retirement note

Exam retired Mar 31 2024; superseded by DP-700 (Microsoft Fabric Data Engineer). This guide is historical and still useful for Azure data engineering concepts.
