# building-database-agent

The `building-database-agent` project explores techniques for interacting with and querying building-related data, including CSV files and SQL databases, using notebooks. The repository provides a step-by-step guide from basic data exploration in CSVs to connecting and querying a SQL database.

## Notebooks Overview

### 1. 01 notebook.ipynb
- **Goal:** Initial exploration of data analysis tools and their usage, likely focusing on basic Python data handling with libraries such as pandas.

### 2. 02 csv_data_interact.ipynb
- **Goal:** Demonstrates how to load CSV files, explore their structure, and interact with their contents.
- **Key Activities:**
  - Reading CSV building data into pandas DataFrames.
  - Exploring the content, such as previewing rows and summarizing columns.
  - Performing sample data manipulations.

### 3. 03 Connecting to SQL Database.ipynb
- **Goal:** Shows how to connect to a SQL database and perform queries on building-related data.
- **Key Activities:**
  - Setting up a connection to a SQL database (such as SQLite, PostgreSQL, etc.).
  - Writing and executing SQL queries to extract, filter, and analyze data.
  - Possibly translating exploratory tasks from the CSV notebook to SQL queries.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/gugrajah/building-database-agent.git
   cd building-database-agent
   ```

2. **Install dependencies:**
   ```
   pip install -r requirements.txt
   ```

3. **Run the notebooks:**
   Open the `.ipynb` files with Jupyter Notebook or a compatible environment to follow along with the data exploration and database interaction demonstrations.

## Directory Structure

- `01 notebook.ipynb` – Introduction to basic data exploration.
- `02 csv_data_interact.ipynb` – Interacting with CSV data.
- `03 Connecting to SQL Database.ipynb` – SQL database connectivity and querying.
- `data/` – Example datasets (if present).
- `requirements.txt` – Python dependencies.

## Requirements

See `requirements.txt` for all Python and notebook dependencies.

---

This project is a practical demonstration of progressing from local CSV data work to leveraging SQL databases for richer, scalable querying—helpful for anyone working with structured building datasets.