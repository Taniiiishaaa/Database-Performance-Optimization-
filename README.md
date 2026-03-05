# Database-Performance-Optimization-
This project is part of the Databases focused on optimizing SQL queries for performance tuning in PostgreSQL 
The project explores how database performance can be improved by analyzing execution plans, designing efficient schemas, and implementing appropriate indexing strategies.

---

# 🎯 Project Objectives

The main goals of this project are:

- Analyze **query execution plans** using PostgreSQL tools
- Design and optimize **database schemas**
- Implement effective **indexing strategies**
- Write **optimized SQL queries**
- Evaluate and compare **query performance**

---

# 📂 Repository Structure
│── 📂 schemas/                   # Database schemas and diagrams
│   ├── Schema-1.png
│   ├── Schema-2.png
│   ├── Schema-4.png
│── 📂 scripts/                    # SQL setup scripts
│   ├── script.sh
│── 📂 queries/                    # SQL queries (original and optimized)
│   ├── original-queries.txt
│   ├── new-queries.txt
│── 📂 docs/                       # Documentation and reports
│   ├── Report.pdf                #Final Report and Documentation of the project
│── 📜 README.md                    # Project introduction and setup guide


---

# 🚀 Getting Started

## 1️⃣ Setting Up the Database

Run the following command to **create the databases and tables**:

```bash
psql -U <your_username> -f scripts/script.sh

2️⃣ Running the Queries
Run the original queries
psql -U <your_username> -d <database_name> -f queries/original-queries.txt
Run the optimized queries
psql -U <your_username> -d <database_name> -f queries/new-queries.txt
3️⃣ Running Performance Analysis

The project report (Report.pdf) includes:

Screenshots of PostgreSQL EXPLAIN ANALYZE output for each query

PostgreSQL configuration and parameter adjustments

Performance comparison between original and optimized queries

Explanation of recommended indexing strategies

📈 Performance Optimization Strategies

Several techniques were used to improve database performance.

🔍 Query Analysis

Used EXPLAIN ANALYZE to inspect query execution plans

Identified expensive operations and bottlenecks

🗂 Indexing Strategies
Index Type	Purpose
B+ Tree Index	Efficient range queries and ordered data
Hash Index	Fast equality lookups
BRIN Index	Optimized for large datasets with sequential values
Mixed Indexing	Combined strategies to improve overall performance
⚡ Query Optimization

Rewrote queries to reduce execution cost

Eliminated unnecessary joins

Reduced scanning of large tables

Optimized filtering conditions

📊 Performance Evaluation

The optimized queries were evaluated based on:

Query execution time

Query execution cost

Index utilization

Improved query execution plans

Results showed significant performance improvements compared to the original queries.

🔧 Dependencies

To run this project you will need:

PostgreSQL 13 or 14

psql CLI

pgAdmin (optional GUI for database management)

📄 Documentation

Detailed analysis and performance comparisons are available in:

docs/Report.pdf

The report includes:

Query analysis results

Execution plan screenshots

Index recommendations

Performance comparison

