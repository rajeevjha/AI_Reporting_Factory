# AI Reporting Factory - Databricks Starter Project

This bundle contains a minimal, runnable starter project for an AI-powered Reporting Factory on Databricks.
It is designed to be run in Databricks notebooks and uses Unity Catalog fully-qualified table names.

Included:
- notebooks/01_modular_etl.ipynb  - Modular ETL (ingest -> enrich -> validate)
- notebooks/02_ai_report_generator.ipynb - Hybrid LLM report generator (natural language + structured)
- notebooks/03_report_export_notify.ipynb - Export views (CSV/Parquet) and notify placeholders
- notebooks/04_dashboard_publisher.ipynb - Automate Databricks SQL dashboard creation via SDK
- metadata/report_definitions.json - metadata template for reports

**IMPORTANT**
- Replace placeholders for OpenAI/LLM keys with secrets stored in Databricks Secret Scopes.
- Some functionality (Databricks SDK calls, model calls) require network and workspace permissions.
- Test notebooks interactively before scheduling as jobs.

