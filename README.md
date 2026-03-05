# Database-Performance-Optimization-
This project is part of the Databases focused on optimizing SQL queries for performance tuning in PostgreSQL 
The project explores how database performance can be improved by analyzing execution plans, designing efficient schemas, and implementing appropriate indexing strategies.

---

# 📖 Overview

Modern database systems require efficient query execution to handle large datasets and high workloads. This project demonstrates how **query performance can be significantly improved** by analyzing execution plans and applying optimization techniques.

The project includes:

- Analysis of **PostgreSQL execution plans**
- Design and evaluation of **database schemas**
- Implementation of **different indexing strategies**
- Development of **optimized SQL queries**
- Performance comparison between **original and optimized queries**

---

# 🎯 Key Features

- 🔍 Query execution plan analysis using **EXPLAIN ANALYZE**
- 📈 SQL performance optimization
- 🗂 Multiple indexing strategies for faster queries
- ⚡ Improved query execution time
- 📊 Performance comparison and evaluation

---

# 📂 Project Structure

```
CSEN604-Database-Optimization-Project/
│
├── schemas/                     # Database schemas and diagrams
│   ├── Schema-1.png
│   ├── Schema-2.png
│   ├── Schema-4.png
│
├── scripts/                     # Database setup scripts
│   ├── script.sh
│
├── queries/                     # SQL queries
│   ├── original-queries.txt     # Original queries
│   ├── new-queries.txt          # Optimized queries
│
├── docs/                        # Project documentation
│   ├── Report.pdf               # Final report and analysis
│
└── README.md                    # Project documentation
```

---

# ⚙️ Installation & Setup

## 1️⃣ Prerequisites

Make sure the following tools are installed:

- **PostgreSQL 13 or 14**
- **psql CLI**
- **pgAdmin** (optional GUI for PostgreSQL)

---

## 2️⃣ Database Setup

Run the following command to create the required database and tables:

```bash
psql -U <your_username> -f scripts/script.sh
```

---

# 🚀 Running the Queries

## Run Original Queries

Execute the original queries to analyze their baseline performance.

```bash
psql -U <your_username> -d <database_name> -f queries/original-queries.txt
```

---

## Run Optimized Queries

Execute the optimized queries to evaluate performance improvements.

```bash
psql -U <your_username> -d <database_name> -f queries/new-queries.txt
```

---

# 📊 Performance Analysis

Query performance was analyzed using PostgreSQL's **EXPLAIN ANALYZE** command.

Example:

```sql
EXPLAIN ANALYZE SELECT * FROM table_name;
```

This command helps identify:

- Sequential scans
- Expensive query operations
- Join inefficiencies
- Index usage

---

# 📈 Optimization Strategies

The following techniques were applied to improve database performance.

## 🔍 Query Execution Plan Analysis

- Used **EXPLAIN ANALYZE** to inspect query execution plans
- Identified expensive operations
- Detected inefficient sequential scans

---

## 🗂 Indexing Strategies

| Index Type | Purpose |
|------------|--------|
| **B+ Tree Index** | Efficient range queries and sorting |
| **Hash Index** | Faster equality lookups |
| **BRIN Index** | Suitable for large datasets with sequential data |
| **Mixed Indexing** | Combination of multiple index strategies |

---

## ⚡ Query Optimization

Optimized queries were written to:

- Reduce full table scans
- Improve filtering conditions
- Optimize joins
- Lower execution cost

---

# 📊 Performance Evaluation

Performance improvements were measured using:

- Query execution time
- Query cost estimation
- Index utilization
- Improved query execution plans

The optimized queries showed **significant improvements in database performance and efficiency** compared to the original queries.

---

# 📄 Documentation

Detailed analysis and results are available in:

```
docs/Report.pdf
```

The report includes:

- Execution plan screenshots
- Query optimization explanations
- Index recommendations
- Performance comparison

--- 

Focus Areas:

- SQL Query Optimization  
- Database Indexing  
- Query Execution Plans  
- PostgreSQL Performance Tuning  

---

