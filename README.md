# Document Preparation Pipeline (Bronze–Silver–Gold)

Cleans and chunks text documents into an embedding-ready format using PySpark and Delta Lake on Databricks.

## Architecture
Raw documents → Bronze (raw ingest) → Silver (cleaned, deduplicated) → Gold (chunked for embedding)

## What it does
- Bronze: raw document ingestion
- Silver: deduplication, cleaning, data quality checks
- Gold: chunks text (~60 words, with overlap) into an embedding-ready table — designed to feed a downstream RAG/LLM pipeline

## Demo
![Summary](your-screenshot-filename.png)
