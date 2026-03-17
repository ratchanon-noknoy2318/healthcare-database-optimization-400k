# HOSxP Analytics Pipeline

SQL-based analytics pipeline for extracting and analyzing operational data from legacy HOSxP hospital systems.

Designed to handle complex relational schemas and enable fast, reliable analytics across hospital departments.

---

## Impact

* Processed **400K+ patient records** across multiple datasets
* Reduced reporting latency from **~24 hours to under 1 hour**
* Enabled cross-department analytics previously limited by schema complexity
* Improved data availability for operational and clinical decision-making
* Used in real-world hospital environments

---

## Problem

HOSxP hospital databases present significant challenges:

* Undocumented and complex relational schemas
* Deep relationships across multiple departments
* High query complexity for cross-functional reporting
* Slow report generation (up to 24 hours)

These limitations made timely analytics and decision-making difficult.

---

## Solution

Designed and implemented a SQL-based analytics pipeline:

* Reverse-engineered legacy database schemas
* Built ETL queries to extract and structure operational data
* Designed optimized query layers for analytics and reporting
* Reduced complexity of multi-table joins
* Improved performance for large-scale data queries

---

## Architecture

Data pipeline flow:

```
[HOSxP MySQL]
        ↓
[SQL ETL Layer]
        ↓
[Analytics Query Layer]
        ↓
[Dashboards / Reports]
```

### Key Considerations

* Optimized query performance for large datasets
* Reduced complexity of multi-table joins
* Ensured data consistency across departments
* Designed for real-world operational usage

---

## Technical Highlights

* Complex SQL joins across multiple relational tables
* Query optimization for large datasets
* Data transformation and aggregation using SQL
* Performance tuning for faster query execution

---

## Challenges

* Working with undocumented legacy database schemas
* Managing complex relationships across hospital systems
* Optimizing slow queries involving large datasets
* Ensuring data correctness in clinical reporting contexts

---

## Tech Stack

* MySQL
* SQL

---

## Project Structure

```
Database/   schema exploration and definitions  
SQL/        ETL and analytics queries  
```

---

## Design Decisions

* **SQL-first approach**

  * Leveraged SQL for both transformation and analytics
  * Reduced system complexity by avoiding unnecessary tooling

* **Optimization over infrastructure**

  * Focused on improving performance within existing systems
  * Avoided introducing additional infrastructure overhead

* **Incremental development**

  * Improved queries iteratively without disrupting production workflows

---

## Future Improvements

* Introduce a data warehousing layer for scalability
* Automate ETL scheduling and orchestration
* Add data validation and monitoring pipelines
* Improve performance for growing datasets

---

## License

MIT
