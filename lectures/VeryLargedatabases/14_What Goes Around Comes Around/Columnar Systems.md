Data management systems that store data column-by-column instead of row-by-row, optimising for analytical workloads.
Architecture:
- [[Data Warehousing (DW)]]
	- Historical data (periodically loaded)
	- Organisations retain everything (TB or PB)
	- [[Queries]] typically only access a small subset of attributes
- Compressing columnar data is more effective
- A [[Volcano-Style Engine]] executes operator once per row. In contrast, a column-oriented engine has an inner loop that processes a whole column using vectorized instructions
- All vendors active in the [[Data Warehousing (DW)]] market have converted their offerings from a row store to a column store
- New actors: Amazon's [[Redshift]] and Google's [[BigQuery]] along with [[Snowflakes]], [[DuckDB]]