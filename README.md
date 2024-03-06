# Analyzing Performance Characteristics of PostgreSQL and MariaDB on NVMeVirt

To understand why the above two database engines have different performance characteristics, we conduct a study of the database engine's internals. We focus on three major differences in Multi-version concurrency control (MVCC) implementations: version storage, garbage collection, and index management.
We also evaluated each scheme's I/O overhead using OLTP workload. Our analysis identifies the reason why MariaDB outperforms PostgreSQL when the bandwidth is low.
