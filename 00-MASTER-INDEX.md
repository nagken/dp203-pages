# DP-203 - Data Engineering on Microsoft Azure Associate - Visual Study Guide

> Concept-only study aid. No exam questions reproduced. Source PDF (if any) stays local + gitignored.

**Skills outline:** https://learn.microsoft.com/credentials/certifications/resources/study-guides/dp-203

## Concept mindmap

```mermaid
mindmap
  root((DP-203))
    Storage Design
      ADLS Gen2 lake zones
      Parquet Delta Avro
      Partitioning pruning
      Distribution hash round-robin replicate
      Star schema SCDs
    Data Processing
      ADF Synapse Pipelines
      Mapping Data Flows
      Spark notebooks
      Stream Analytics windows
      Event time watermarks IR triggers
    Secure Monitor Optimize
      Encryption TDE CMK
      RLS CLS DDM ACLs
      Managed Identity Key Vault Purview
      Azure Monitor Log Analytics KQL
      Statistics small files skew
```

## Domain map

```mermaid
flowchart LR
    Master["DP-203 Master Index"]
    D01["Design and Implement Data Storage"]
    Master --> D01
    D02["Develop Data Processing"]
    Master --> D02
    D03["Secure Monitor and Optimize Data"]
    Master --> D03
```

## Domain weights

```mermaid
pie showData
    title DP-203 domain weights
    "Design and Implement Data Storage" : 42
    "Develop Data Processing" : 35
    "Secure Monitor and Optimize Data" : 23
```

> Click a slice / legend label to jump to that chapter.

## Recommended study order

```mermaid
gantt
    title Suggested study plan
    dateFormat X
    axisFormat Day %d
    section Plan
    Design and Implement Data Storage :t1, 0, 2d
    Develop Data Processing :t2, after t1, 2d
    Secure Monitor and Optimize Data :t3, after t2, 1d
```

---

**Next:** open [01-design-implement-storage.md](01-design-implement-storage.md)

<!-- TODO: fill remaining sections via Copilot chat. Target structure mirrors c:\az305\study-guide\00-MASTER-INDEX.md. -->
