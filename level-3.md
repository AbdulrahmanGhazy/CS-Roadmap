## DataBase :

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

- From SQL  ****———To ———>   [**Solution To: "Saving changes is not permitted" error ]**

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

## OS (Operating System) :
Course playList : https://www.youtube.com/watch?v=NyWYS7pUer0&list=PLSGEGD0dbMKoigQWgVJ_UoUJUGQPCHXKV

A 7-week self-paced roadmap to build a solid understanding of Operating Systems. Weeks 1–6 follow one video per week from the OS playlist. Week 7 covers Linux basics.

---

## Week 1: Introduction to Operating Systems and Computer System Organization

Videos :

- Introduction to Operating Systems and Computer System Organization

Key concepts: operating system as an intermediary between hardware and applications, kernel, bootstrap program and firmware, device controllers, interrupts and the interrupt vector, storage hierarchy, caching and cache coherency, interrupt-driven I/O versus DMA, multiprocessor systems, graceful degradation, clusters.

Task:
Explain the concepts in your own words

1. What is an operating system and why do we need one? Explain it with your own analogy, and mention the role of the hardware, the OS, and the application.
2. A user touches the touchpad while a program is running. Explain step by step what happens until the CPU returns to the original program, and mention the interrupt, the interrupt vector, and the interrupt service routine.
3. What is the difference between interrupt-driven I/O and DMA? Explain which one is better for a high-speed network card and why.

---

## Week 2: Operating System Operations

Videos :

- Operating System Operations

Key concepts: dual-mode operation (user mode and kernel mode), privileged instructions, timer, batch systems, multiprogramming and time-sharing, computing environments (mobile, networks, distributed systems, client-server, peer-to-peer), virtualization, cloud computing, embedded and real-time systems.

Task:

Explain the concepts in your own words

1. Why does the OS need two modes of operation (user mode and kernel mode)? Explain what the mode bit does when an application tries to run a privileged instruction, and how the timer prevents one program from keeping the CPU forever.
2. What is the difference between a batch system, a multiprogramming system, and a time-sharing system? Explain why multiprogramming keeps the CPU busier, and what time-sharing adds for interactive users.
3. What is virtualization and why is it useful? Then explain why a website that gets huge traffic only one day a year (like an exam results website) benefits from cloud computing more than from a fixed hosting plan.

---

## Week 3: Operating System Structures

Videos :

- OS Services, System Calls, OS Structure and Process Concept

Key concepts: OS services, system calls and API, parameter passing (registers, memory block, stack), system programs, OS structures (monolithic, layered, microkernel, loadable modules), process in memory (text, data, stack, heap), process states, Process Control Block (PCB), context switch, ready queue, process creation.

Task:
Explain the concepts in your own words

1. What is a system call, and why do programmers use an API instead of calling system calls directly? Explain the three ways of passing parameters to a system call.
2. Compare the layered approach and the microkernel approach in OS design. Mention one advantage and one disadvantage of each.
3. What are the parts of a process in memory (text, data, stack, heap) and what is each one used for? Then explain what a context switch is and why it is considered overhead.

---

## Week 4: Process Synchronization and Deadlocks

Videos :

- Process Synchronization and Deadlocks

Key concepts: producer-consumer problem, race condition, critical section, requirements of a solution (mutual exclusion, progress, bounded waiting), hardware support (test_and_set, compare_and_swap), mutex locks, semaphores, busy waiting, deadlock and its four conditions, resource-allocation graph, deadlock handling (ignore, prevention/avoidance, detection and recovery), lock ordering.

Task:
Explain the concepts in your own words

1. What is a race condition? Using the producer-consumer example (count++ and count--), explain how it can lead to a wrong value of count, and what a critical section is.
2. What are the three requirements for a correct critical-section solution (mutual exclusion, progress, bounded waiting)? Explain each one with a simple example, like the restroom analogy.
3. What is a deadlock, and what are its four necessary conditions? Explain why lock ordering (acquiring locks in the same order) prevents deadlock.

---

## Week 5: CPU Scheduling

Videos :

- CPU Scheduling

Key concepts: CPU scheduler and dispatcher, preemptive vs non-preemptive scheduling, scheduling criteria (CPU utilization, throughput, turnaround time, waiting time, response time), FCFS and convoy effect, SJF and SRTF, priority scheduling (starvation and aging), Round Robin and time quantum.

Task:
Explain the concepts in your own words

1. What is the difference between turnaround time, waiting time, and response time? Then explain the convoy effect in FCFS and how SJF solves it, and why SJF is hard to implement in practice.
2. What is starvation in priority scheduling and how does aging solve it? Then explain how Round Robin works and what the time quantum affects.
3. What is the difference between preemptive and non-preemptive scheduling? Give one example of an algorithm for each, and explain when the scheduler has to make a decision.

---

## Week 6: Memory Management

Videos :

- Memory Management

Key concepts: logical vs physical address, address binding (compile time, load time, execution time), MMU, base and limit registers, swapping and backing store, contiguous allocation (first-fit, best-fit, worst-fit), external and internal fragmentation, compaction, paging (frames, pages, page table), shared pages, segmentation.

Task:
Explain the concepts in your own words

1. What is the difference between a logical address and a physical address? Explain the three times when address binding can happen (compile time, load time, execution time) and what the MMU does.
2. What are first-fit, best-fit, and worst-fit in contiguous memory allocation? Then explain the difference between external fragmentation and internal fragmentation, with one example of each.
3. How does paging solve external fragmentation? Explain how a logical address is translated into a physical address using the page number, the offset, and the page table.

---

## Week 7: Introduction to Linux Command Line & Shell Fundamentals

Videos :
•    Learn Command Line 

Key concepts: Terminal vs Shell vs CLI, standard Linux directory hierarchy, shell navigation, file and directory management, viewing and editing content, I/O redirection, pipes, searching and text processing, permissions and ownership.

Task:
Practice the commands in a Linux terminal

1. Using a single command, create the directory tree `project/src` and `project/logs` in your home directory. Then go to `project/logs` and create three files: `app.log`, `error.log`, and `system.log`.
2. From inside `project/logs`, append the text "ERROR 404: Page not found" to `error.log` and "INFO: Server started successfully" to `app.log`. Then search for the word "ERROR" in all files inside the `logs` directory and save the matching lines in a new file named `filtered_errors.txt` inside the `project` directory (not inside `logs`).
3. Use `cat` and `grep` with a pipe (`|`) to display only the line containing "INFO" from `app.log`. Then change the permissions of `filtered_errors.txt` so that only the owner can read and write it (no permissions for group or others).

Submit the commands you used and a screenshot of the terminal output.
