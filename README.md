# Building A Database Agent

The `building-database-agent` project explores techniques for interacting with and querying building-related data, including CSV files and SQL databases, using notebooks. The repository provides a step-by-step guide from basic data exploration in CSVs to connecting and querying a SQL database, and ultimately building an AI-powered natural language interface using Azure OpenAI's function calling capabilities.

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

### 4. 04 Azure OpenAI Function Calling Feature.ipynb
- **Goal:** Demonstrates how to use Azure OpenAI's function calling capabilities to create an intelligent agent that can interact with databases using natural language queries.
- **Key Activities:**
  - **Setup:** Configuring Azure OpenAI client with proper credentials and API endpoints.
  - **Illustrative Example:** Building a weather function calling system to demonstrate the basic concept of function calling with Azure OpenAI, including:
    - Defining custom functions (e.g., `get_current_weather`)
    - Creating tool definitions with proper JSON schemas
    - Handling multiple function calls in a single conversation
  - **SQL Database Integration:** Applying function calling to real database queries:
    - Creating a SQLite database from COVID-19 tracking data (`all-states-history.csv`)
    - Implementing database query functions (`get_hospitalized_increase_for_state_on_date`, `get_positive_cases_for_state_on_date`)
    - Defining tools that allow the AI to intelligently query the database based on user questions
    - Processing natural language queries like "how many hospitalized people we had in Alaska on 2021-03-05?" and automatically calling the appropriate database functions
    - Handling function responses and generating human-readable answers from database results

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
- `04 Azure OpenAI Function Calling Feature.ipynb` – AI-powered natural language database querying with Azure OpenAI.
- `data/` – Example datasets.
- `requirements.txt` – Python dependencies.

## Requirements

See `requirements.txt` for all Python and notebook dependencies.

---

This project is a practical demonstration of progressing from local CSV data work to leveraging SQL databases for richer, scalable querying—helpful for anyone working with structured building datasets.
