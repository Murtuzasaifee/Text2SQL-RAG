# Text2SQL-RAG

A project exploring Text-to-SQL capabilities using Retrieval-Augmented Generation (RAG) with LlamaIndex and OpenAI. This repository contains a progression of notebooks from basic to advanced implementations, culminating in a live PostgreSQL (Supabase) integration.

## Features

- **Progressive Learning**: Step-by-step notebooks covering basic to advanced Text-to-SQL techniques.
- **RAG Integration**: Leverages LlamaIndex for enhanced context and query generation.
- **Vanna.ai Integration**: Comprehensive tutorial on using Vanna.ai 2.0 Agent Framework for Text-to-SQL.
- **Database Support**: Includes examples for local databases (DuckDB) and production-ready PostgreSQL (Supabase).
- **Utility Scripts**: Tools for connection testing and sample data generation.

## Setup

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd Text2SQL-RAG
   ```

2. **Install dependencies:**
   This project uses `uv` for dependency management.
   ```bash
   uv sync
   ```
   Or using pip:
   ```bash
   pip install -r pyproject.toml
   ```

3. **Environment Configuration:**
   Create a `.env` file based on your credentials:
   ```env
   OPENAI_API_KEY=your_key_here
   POSTGRES_USER=your_user
   POSTGRES_PASSWORD=your_password
   POSTGRES_HOST=your_host
   POSTGRES_DB=your_db
   ```

4. **Run the Notebooks:**
   Explore the `notebooks/` directory starting with `01_basic_text_to_sql.ipynb`.

## Project Structure

- `notebooks/`: Interactive tutorials (Basic, Intermediate, Advanced, PostgreSQL, Vanna.ai).
- `setup_supabase_schema.sql`: SQL schema for the target data structure.
- `create_sample_tables.py`: Script to seed sample data into Supabase/Postgres.
- `test_supabase_connection.py`: Verify database connectivity.
