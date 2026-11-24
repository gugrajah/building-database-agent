# Natural-Language SQL & Database Agent

An agentic AI workflow that bridges the gap between non-technical stakeholders and relational databases—translating plain-English business questions into accurate, schema-aware SQL queries and concise analytical summaries.

### Business & Architectural Problem
Ad-hoc data requests frequently bottleneck analytics teams, while giving business users raw database access risks malformed queries and misread metrics. This agent inspects database schemas dynamically, generates grounded SQL queries, executes them safely, and synthesizes the output into decision-ready context.

### Key Capabilities
* **Schema-Aware Query Generation:** Introspects table structures and relationships before drafting SQL to minimize hallucinated column names or invalid joins.
* **Self-Correcting Execution Loop:** Captures SQL syntax or execution errors and iteratively refines the query before returning results.
* **Human-Readable Synthesis:** Converts raw tabular query outputs into clear, plain-language takeaways tailored to the original business question.
