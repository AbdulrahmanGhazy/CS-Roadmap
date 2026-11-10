This plan follows the Programming Advices course "Database Level 1 - SQL (Concepts and Practice)"

---

## Week 1: Concepts and ERD Basics (about 3.5 hours of video)

Videos : 

- From [ **Installing SQL Sever 2022 ]**  ———To ———  **Database Design: Conceptual Design  [Relationships]**

**Key concepts:** database versus data structure, `NULL`, primary and foreign keys, redundancy, integrity, constraints, ERD symbols, strong and weak entities.

**Weekly task: Concepts and a first ERD**

1. Write a one-line definition in your own words for: database, `NULL`, primary key, foreign key, redundancy, data integrity, constraint.
2. Install SQL Server 2022 and SSMS.
3. Draw a first ERD for a small library (books, members, loans) with entities, attributes and relationships, using the symbols from the lectures.

---

## Week 2: ERD Advanced and Relational Schema (about 3.9 hours of video)

Videos : 

- From **Database Design: Conceptual Design  [One-to-One Relationship]**  ———To ———>  **Relational Schema  [How to create Relational Schema on ERDPlus.com? ]**

**Key concepts:** relationship types, cardinality and participation, associative entities, generalization and specialization, the rules for turning each ERD shape into tables.

**Weekly task: ERD to relational schema**

1. Follow the step-by-step small project lecture to draw a complete ERD for a university or online store with at least one many-to-many relationship.
2. Mark cardinality and participation on every relationship.
3. Convert it to a relational schema (tables, columns, primary keys, foreign keys), by hand and on ERDPlus.com.
4. Keep this schema; you build it in Week 3.

---

## Week 3: Build the Database: DDL, Backup and DML (about 2.7 hours of video)

Videos : 

- From SQL  ———To ———>   [**Solution To: "Saving changes is not permitted" error ]**

**Key concepts:** `CREATE` / `ALTER` / `DROP`, data types, backup and restore, `INSERT` / `UPDATE` / `DELETE`, identity columns, `DELETE` versus `TRUNCATE`, foreign keys.

**Weekly task: Turn your design into a real database**

1. Create the database and every table from your Week 2 relational schema, with identity primary keys and foreign keys.
2. Insert at least 10 rows into each table, parents before children.
3. Try to insert a child row with a missing parent and read the error.
4. Use `ALTER TABLE` to add one column and rename another.
5. Take a full backup, change some data, then restore it.
6. Run a `SELECT` with the same `WHERE` before every `UPDATE` and `DELETE`.

---

## Week 4: Queries, Joins and Views (about 2.9 hours of video)

Videos : 

- From SQL - Queries ———To ———> **SQL - More Queries [ Case ]**

**Key concepts:** filtering, sorting, aliases, aggregates, `WHERE` versus `HAVING`, wildcards, inner versus outer joins, views, `EXISTS`, `UNION`, `CASE`.

**Weekly task: 25 queries**

1. On the sample HR database, write 10 queries (filters, sorting, top rows, aggregates, `GROUP BY` with `HAVING`).
2. On the Shop database, write 10 join queries (customers with their orders, customers with no orders, totals per customer).
3. On your own database from Week 3, write 5 queries and create one view.

---

## Week 5: Constraints, Indexes and Normalization (about 1.5 hours of video, more practice)

Videos : 

- From **Constraints** ———To ———> End of Course

**Weekly task: Harden and normalize**

1. Add `DEFAULT`, `CHECK`, `UNIQUE` and `NOT NULL` constraints to your Week 3 tables where they make sense.
2. Create an index on a column you search often, and explain in a sentence why it helps.
3. Create one deliberately messy table (for example an orders table that repeats customer data) and normalize it step by step to 3NF.

---

## Week 6: Final Project, Design to Queries

Note : Rewatch the two or three lectures on the topics you found hardest.

Build the project below.

**Final project (library or online store)**

1. Requirements: write what the system must store and answer.
2. Design: ERD, then relational schema, then normalize to 3NF.
3. Build: 5-6 tables with all constraints, an index, and 50+ rows of sample data.
4. Query: 15+ queries using joins, grouping and window functions.
5. Program: 2 views, 3 stored procedures, one trigger and one transaction with rollback.
6. Back up the finished database.

---
