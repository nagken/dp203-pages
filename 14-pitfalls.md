# DP-203 Pitfalls

Mistakes that lose easy points on the exam.

- Round-robin large facts - kills join perf.
- Low-cardinality partitions - skew + small files.
- Pay-while-paused dedicated SQL pool for tiny workloads.
- Type 2 SCD without effective dates.
- Processing time when event time matters.
- Hopping where tumbling would do.
- Long-lived account keys instead of MI.
- DDM treated as actual security.
- Forgetting UPDATE STATISTICS after bulk loads.
- Missing Git integration for pipelines.
