# DP-203 Flashcards

Click each card to flip.

<section class="fc-section" data-fc-title="Design and Implement Data Storage">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: When pick serverless over dedicated SQL pool?</div><div class="fc-a">A: Ad-hoc, low/intermittent usage; pay only per query. Dedicated = steady-state warehouse.</div></div>
<div class="flashcard"><div class="fc-q">Q: Hash distribution best when?</div><div class="fc-a">A: Large fact tables joining on high-cardinality columns.</div></div>
<div class="flashcard"><div class="fc-q">Q: Round-robin best for?</div><div class="fc-a">A: Staging/loading tables - even but no co-location.</div></div>
<div class="flashcard"><div class="fc-q">Q: Replicate best for?</div><div class="fc-a">A: Small dimensions (<2GB) - copied to every compute node.</div></div>
<div class="flashcard"><div class="fc-q">Q: Type 2 SCD vs Type 1?</div><div class="fc-a">A: Type 2 keeps history (new row per change); Type 1 overwrites.</div></div>
<div class="flashcard"><div class="fc-q">Q: Why Parquet for analytics?</div><div class="fc-a">A: Columnar + compressed + predicate pushdown - much faster column scans.</div></div>
<div class="flashcard"><div class="fc-q">Q: What is Delta Lake?</div><div class="fc-a">A: Parquet + transaction log = ACID, upserts, time travel on data lake.</div></div>
</div>
</section>

<section class="fc-section" data-fc-title="Develop Data Processing">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: Tumbling vs hopping window?</div><div class="fc-a">A: Tumbling = non-overlapping fixed intervals. Hopping = fixed size with hop period (overlapping).</div></div>
<div class="flashcard"><div class="fc-q">Q: Event time vs processing time?</div><div class="fc-a">A: Event time from event itself; processing time at processor. Event time correct for analytics.</div></div>
<div class="flashcard"><div class="fc-q">Q: When use Stream Analytics over Spark Structured Streaming?</div><div class="fc-a">A: SQL-like simple streaming, low-code, integrated with Event Hubs. Spark for complex transforms / ML.</div></div>
<div class="flashcard"><div class="fc-q">Q: Mapping Data Flows engine?</div><div class="fc-a">A: Spark cluster managed for you by ADF/Synapse.</div></div>
<div class="flashcard"><div class="fc-q">Q: Integration Runtime types?</div><div class="fc-a">A: Azure (cloud), Self-hosted (on-prem), Azure-SSIS.</div></div>
<div class="flashcard"><div class="fc-q">Q: How handle late-arriving stream events?</div><div class="fc-a">A: Watermarks + allowed lateness on the window.</div></div>
</div>
</section>

<section class="fc-section" data-fc-title="Secure, Monitor, and Optimize Data">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: Managed identity vs service principal?</div><div class="fc-a">A: MI has no secret to manage and is tied to the resource lifecycle. SP requires secret/cert mgmt. Prefer MI.</div></div>
<div class="flashcard"><div class="fc-q">Q: TDE encrypts what?</div><div class="fc-a">A: Data at rest at the SQL data + log + backup level - transparent to queries.</div></div>
<div class="flashcard"><div class="fc-q">Q: RLS vs CLS?</div><div class="fc-a">A: RLS filters which rows you see (security predicate). CLS controls which columns you can SELECT.</div></div>
<div class="flashcard"><div class="fc-q">Q: Why compact small files in the lake?</div><div class="fc-a">A: Each file has open/scan overhead - many small files destroys Spark/SQL perf.</div></div>
<div class="flashcard"><div class="fc-q">Q: Where statistics live in dedicated SQL pool?</div><div class="fc-a">A: Per-table; updated automatically but UPDATE STATISTICS after bulk loads to keep current.</div></div>
<div class="flashcard"><div class="fc-q">Q: Purview job-to-be-done?</div><div class="fc-a">A: Catalog + classify + trace lineage of data assets across estate.</div></div>
</div>
</section>
