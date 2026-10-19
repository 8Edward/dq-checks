# dq-checks

dq-checks is a small Python library and CLI for data quality checks.
You describe checks in a YAML config (not null, unique, accepted values,
row count, freshness), and dq-checks runs them as SQL queries against
PostgreSQL or ClickHouse. It prints a report and exits with a non-zero
code when a check fails, so an orchestrator like Airflow can stop the pipeline.

## Project structure

- `src/dq_checks/` — Python package: data quality checks and CLI
- `tests/` — pytest tests
