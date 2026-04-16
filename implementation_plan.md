# 🗄️ Database Mastery — إتقان قواعد البيانات
## Complete Implementation Plan: Zero to Hero Database Learning Platform

---

> [!IMPORTANT]
> This is a **standalone, masterpiece-level educational platform** — a sibling project to your existing Algorithms platform. It follows the same proven interactive HTML approach with glass-morphism design, Egyptian Arabic explanations, and hands-on interactivity, but now for **Databases from Zero to Hero**.

---

## 🎯 Vision & Philosophy

**A world-class, self-contained platform that takes any student — whether a first-year CS student at Cairo University or someone learning for a career change — from knowing absolutely nothing about databases to mastering them at an industry-ready level.**

### Target Audience (Dual-Track)
| Track | Who | What They Need |
|-------|-----|---------------|
| 🎓 **Academic Track** | CS/IT students at Egyptian universities (FCIS Ain Shams, FCAI Cairo, FCDS Alexandria, GUC, AAST, etc.) | Aligns with Elmasri & Navathe textbook, covers ER diagrams, relational algebra, normalization theory, transaction processing — everything in their exams |
| 💼 **Career Track** | Self-learners, career changers, bootcamp students wanting backend/data roles | Practical SQL, ORM usage (Prisma), real API building (NestJS/Express), portfolio projects, interview prep |

### Design Principles
- **Units, not weeks** — no timeline pressure, learn at your own pace
- **Egyptian Arabic explanations** with English technical terms
- **Every concept has an interactive visualization** — not just text
- **Live SQL playground** in every SQL lesson — write and execute queries in the browser
- **Real backend projects** using express and NestJS (advanced) + PostgreSQL + Prisma
- **Progressive difficulty** — each unit builds on the previous

---

## 📊 Existing Project Analysis

Your algorithms project establishes excellent patterns we will replicate and enhance:

### Architecture Patterns to Reuse
| Pattern | From Algorithms | Enhanced For Database |
|---------|----------------|----------------------|
| **Portal page** | `index.html` with aurora blobs, particle canvas, card grid | Same but with 10 unit cards instead of 4 weeks |
| **Lesson structure** | Hero → Concept → Step-by-step → Interactive Demo → Code | Hero → Concept → Step-by-step → **SQL Playground** → Code → **Mini-Project** |
| **Bilingual content** | Arabic explanations + English terms | Same approach |
| **Glass-morphism design** | `glass-card`, dark theme, gradient accents | Same design system, different color palette (emerald/amber for DB) |
| **Interactive visualizations** | Canvas-based algorithms | Canvas + **live SQL execution** + **ER diagram builders** + **table visualizers** |
| **Scripts directory** | El Daheeh-style teaching scripts | Same for video production |
| **Tasks directory** | Hands-on practice exercises | **Expanded with real backend projects** |
| **Notification system** | Contextual tips | Same system |

### New Capabilities Added
- 🔴 **In-browser SQL Playground** (using sql.js / PGlite for client-side PostgreSQL)
- 🔴 **ER Diagram Builder** (interactive drag-and-drop)
- 🔴 **Schema Visualizer** (shows tables, relationships, constraints live)
- 🔴 **NestJS/Prisma Code Labs** (guided backend project building)
- 🔴 **Query Optimizer Visualizer** (shows EXPLAIN ANALYZE results visually)

---

## 🏗️ Tech Stack

### Frontend (Interactive Lessons)
| Technology | Purpose |
|-----------|---------|
| **HTML5 + Vanilla CSS + JavaScript** | Standalone lesson pages (same as algorithms) |
| **TailwindCSS CDN** | Utility classes for rapid UI (same as algorithms lessons) |
| **Canvas API** | Custom visualizations (ER diagrams, B-trees, etc.) |
| **PGlite / sql.js** | In-browser PostgreSQL/SQLite for live SQL playground |
| **AOS.js** | Scroll animations |
| **Font Awesome** | Icons |
| **Cairo + Inter + Fira Code** | Fonts (Arabic + English + Code) |

### Backend (Project Labs & API)
| Technology | Purpose |
|-----------|---------|
| **expressjs and NestJS (advanced)** | Main backend framework (taught in Unit 6+) |
| **PostgreSQL** | Primary database (taught throughout) |
| **Prisma ORM** | Database toolkit & ORM (taught in Unit 6+) |
| **Docker** | Database containerization for easy setup |

---

## 📚 Complete Curriculum — 10 Units

---

### 🟢 UNIT 1: عالم قواعد البيانات — The World of Databases
**Level:** Absolute Beginner | **Lessons:** 5 | **Color:** `#10B981` (Emerald)

> *"قبل ما نكتب أي كود، لازم نفهم ليه العالم محتاج قواعد البيانات أصلاً"*

#### Lesson 1.1: `why_databases.html` — ليه محتاجين قواعد بيانات؟
- **Concept:** The problem with files — data redundancy, inconsistency, isolation
- **Visualization:** Interactive animation showing a school storing student data in Excel sheets vs. a database
- **Real-world analogy:** "تخيل مكتبة فيها مليون كتاب من غير فهرس" 📚
- **Egyptian context:** Registration systems at Egyptian universities as an example

#### Lesson 1.2: `database_types.html` — أنواع قواعد البيانات
- **Concept:** Relational vs. NoSQL vs. Graph vs. Time-Series vs. Key-Value
- **Visualization:** Interactive comparison cards — click each type to see real-world examples
- **Content:** When to use what (Facebook uses both MySQL AND Cassandra AND TAO)
- **Career context:** Which databases Egyptian companies use (Vodafone Egypt → Oracle, Instapay → PostgreSQL, etc.)

#### Lesson 1.3: `database_architecture.html` — معمارية قواعد البيانات
- **Concept:** Three-Schema Architecture (External, Conceptual, Internal)
- **Visualization:** Interactive 3-layer diagram — click each layer to explore
- **Academic content:** Data independence (logical & physical) — exam-essential for FCIS/FCAI students
- **DBMS components breakdown:** Query processor, storage manager, transaction manager

#### Lesson 1.4: `postgresql_setup.html` — تثبيت PostgreSQL
- **Concept:** Installing PostgreSQL + pgAdmin + psql
- **Content:** Step-by-step guide with screenshots for Windows/Mac/Linux
- **Docker setup:** Alternative using Docker for quick start
- **First commands:** `CREATE DATABASE`, `\l`, `\dt`, `\d`
- **Interactive:** Terminal simulator showing psql commands

#### Lesson 1.5: `database_history.html` — تاريخ قواعد البيانات
- **Concept:** From file systems (1960s) → Hierarchical (IMS) → Network (CODASYL) → Relational (Codd, 1970) → Object-Oriented → NoSQL → NewSQL
- **Visualization:** Interactive timeline with milestones
- **Tribute:** Edgar F. Codd's 12 rules, Ramez Elmasri's contributions (Egyptian-American!)
- **Fun fact:** The word "SQL" was originally "SEQUEL" by IBM

---

### 🔵 UNIT 2: النموذج العلائقي و ER Diagrams — Data Modeling
**Level:** Beginner | **Lessons:** 5 | **Color:** `#3B82F6` (Blue)

> *"قبل ما تبني بيت، لازم ترسم المخطط — وقبل ما تبني Database، لازم ترسم الـ ER Diagram"*

#### Lesson 2.1: `er_basics.html` — أساسيات الـ ER Diagram
- **Concept:** Entities, Attributes, Relationships
- **Visualization:** **Interactive ER Diagram Builder** — drag entities, add attributes, connect relationships
- **Example:** University database (Student, Course, Professor, Department)
- **Academic:** Strong vs. Weak entities, key attributes, derived attributes, multi-valued attributes

#### Lesson 2.2: `er_relationships.html` — العلاقات في ER
- **Concept:** One-to-One, One-to-Many, Many-to-Many, cardinality, participation constraints
- **Visualization:** Interactive relationship explorer — change cardinality and see the diagram update
- **Examples:** 
  - 1:1 → "الطالب وبطاقته الجامعية"
  - 1:N → "القسم والموظفين"  
  - M:N → "الطلاب والمواد"
- **Academic:** Total vs. Partial participation, (min,max) notation

#### Lesson 2.3: `eer_diagrams.html` — الـ EER المتقدم
- **Concept:** Specialization, Generalization, Union types, Categories
- **Visualization:** Interactive EER builder with inheritance hierarchies
- **Examples:** Vehicle → (Car, Truck, Motorcycle) specialization
- **Academic:** Disjoint vs. Overlapping, Total vs. Partial specialization — critical for exams

#### Lesson 2.4: `relational_model.html` — النموذج العلائقي
- **Concept:** Relations (tables), Tuples (rows), Attributes (columns), Domains, Keys
- **Visualization:** Interactive table builder — create a relation and see its properties
- **Keys deep-dive:** Super Key → Candidate Key → Primary Key → Foreign Key → Composite Key
- **Relational Algebra:** σ (select), π (project), × (cross product), ⋈ (join), ∪, ∩, −
- **Interactive:** Drag-and-drop relational algebra operations on sample tables

#### Lesson 2.5: `er_to_relational.html` — تحويل ER إلى Tables
- **Concept:** Step-by-step mapping algorithm (7 steps from Elmasri & Navathe)
- **Visualization:** Animated transformation — watch an ER diagram become tables before your eyes
- **Steps:** Map strong entities → weak entities → 1:1 → 1:N → M:N → multi-valued → n-ary
- **Interactive quiz:** Given an ER diagram, create the correct tables

---

### 🟡 UNIT 3: أساسيات SQL — SQL Fundamentals
**Level:** Beginner → Intermediate | **Lessons:** 5 | **Color:** `#F59E0B` (Amber)

> *"SQL هي اللغة اللي بتتكلم بيها مع الـ Database — وهي أهم مهارة في عالم البيانات"*

#### Lesson 3.1: `ddl_basics.html` — إنشاء الجداول (DDL)
- **SQL Playground:** Live in-browser SQL execution
- **Commands:** `CREATE TABLE`, `ALTER TABLE`, `DROP TABLE`, `TRUNCATE`
- **Data Types:** INTEGER, VARCHAR, TEXT, BOOLEAN, DATE, TIMESTAMP, NUMERIC, SERIAL, UUID
- **Constraints:** `PRIMARY KEY`, `FOREIGN KEY`, `NOT NULL`, `UNIQUE`, `CHECK`, `DEFAULT`
- **Exercises:** Build the University database from Unit 2's ER diagram

#### Lesson 3.2: `dml_crud.html` — عمليات CRUD
- **SQL Playground:** Live editing with instant results
- **Commands:** `INSERT INTO`, `SELECT`, `UPDATE`, `DELETE`
- **Filtering:** `WHERE`, `AND`, `OR`, `NOT`, `IN`, `BETWEEN`, `LIKE`, `IS NULL`
- **Sorting & Limiting:** `ORDER BY`, `LIMIT`, `OFFSET`
- **Exercises:** 15+ progressive exercises with auto-checking

#### Lesson 3.3: `aggregate_grouping.html` — التجميع والتصنيف
- **SQL Playground:** Aggregate queries with visual results
- **Functions:** `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`
- **Grouping:** `GROUP BY`, `HAVING`
- **Visualization:** Bar charts that update as you write GROUP BY queries
- **Real example:** "احسب متوسط درجات كل طالب في كل مادة"

#### Lesson 3.4: `joins_mastery.html` — إتقان الـ Joins
- **Concept:** The most important SQL topic — connecting tables
- **Visualization:** **Venn diagram animator** — see exactly which rows each JOIN returns
- **Types:** `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL OUTER JOIN`, `CROSS JOIN`, `SELF JOIN`
- **SQL Playground:** Side-by-side tables with JOIN results
- **Visual:** Animated rows flying from one table to another during a JOIN
- **Exercises:** 10 progressive JOIN challenges

#### Lesson 3.5: `subqueries_sets.html` — الاستعلامات الفرعية
- **Concept:** Subqueries (scalar, row, table), correlated subqueries
- **Set Operations:** `UNION`, `INTERSECT`, `EXCEPT`
- **`EXISTS` vs `IN`:** Performance comparison with visualization
- **SQL Playground:** Write nested queries with step-by-step execution visualization
- **Challenge:** "اعرض الطلاب اللي درجاتهم أعلى من المتوسط في كل مادة"

---

### 🟠 UNIT 4: SQL المتقدم — Advanced SQL
**Level:** Intermediate | **Lessons:** 4 | **Color:** `#F97316` (Orange)

> *"دلوقتي بقيت تعرف SQL — لكن فيه حاجات قوية جداً لسه ما اتعلمتهاش"*

#### Lesson 4.1: `views_ctes.html` — Views و CTEs
- **Views:** `CREATE VIEW`, updatable views, materialized views
- **CTEs:** `WITH` clause for readable complex queries
- **Recursive CTEs:** `WITH RECURSIVE` for hierarchical data (organization charts, categories)
- **SQL Playground + Visualization:** See the virtual table a VIEW creates

#### Lesson 4.2: `window_functions.html` — Window Functions
- **Concept:** Analytics without losing row detail
- **Functions:** `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, `NTILE()`, `LAG()`, `LEAD()`
- **`OVER()` clause:** `PARTITION BY`, `ORDER BY`, window frames (`ROWS BETWEEN`)
- **Visualization:** Animated sliding window over table rows
- **Real use case:** "رتب الطلاب حسب درجاتهم في كل قسم"

#### Lesson 4.3: `advanced_types.html` — أنواع بيانات متقدمة في PostgreSQL
- **JSONB:** Storing and querying JSON data (`->`, `->>`, `@>`, `?`)
- **Arrays:** PostgreSQL array types and operations
- **ENUM types:** Custom enumeration types
- **Date/Time functions:** `EXTRACT`, `DATE_TRUNC`, `AGE`, intervals
- **Full-text search:** `tsvector`, `tsquery`, `to_tsvector()`
- **SQL Playground:** Experiment with each data type

#### Lesson 4.4: `functions_triggers.html` — Functions و Triggers
- **PL/pgSQL:** Writing stored functions and procedures
- **Triggers:** `BEFORE`/`AFTER` triggers for `INSERT`/`UPDATE`/`DELETE`
- **Use case:** Audit trail — automatically log every change to a table
- **SQL Playground:** Write and test your own functions
- **Interactive:** Watch a trigger fire in real-time when you insert data

---

### 🟣 UNIT 5: تصميم قواعد البيانات والتطبيع — Database Design & Normalization
**Level:** Intermediate (Academic-Heavy) | **Lessons:** 4 | **Color:** `#8B5CF6` (Purple)

> *"ده الـ Unit اللي بيفرق بين حد بيستخدم Database وحد بيصمم Database"*

> [!NOTE]
> This unit is **critical for university exams** at FCIS, FCAI, FCDS. It covers exactly what Elmasri & Navathe Chapters 14-15 teach.

#### Lesson 5.1: `functional_dependencies.html` — الاعتمادات الوظيفية
- **Concept:** What is a Functional Dependency (FD)? Notation: X → Y
- **Armstrong's Axioms:** Reflexivity, Augmentation, Transitivity
- **Closure of attributes:** Computing X⁺
- **Visualization:** Interactive FD graph — add dependencies and compute closures
- **Candidate key finder:** Algorithm to find all candidate keys from FDs

#### Lesson 5.2: `normalization.html` — التطبيع (Normalization)
- **Normal Forms:** 1NF → 2NF → 3NF → BCNF → 4NF → 5NF
- **Visualization:** **Animated decomposition** — watch a table split into normalized forms
- **Step-by-step:** Identify violations → Decompose → Verify
- **Examples with Egyptian context:** 
  - "جدول الطلاب اللي فيه مشاكل" → normalize step by step
- **Interactive quiz:** "هل الجدول ده في 3NF ولا لأ؟"

#### Lesson 5.3: `denormalization.html` — عكس التطبيع (Denormalization)
- **Concept:** When and why to denormalize
- **Trade-offs:** Read performance vs. data integrity
- **Real-world examples:** Facebook's denormalized friend lists, e-commerce product pages
- **Visualization:** Performance comparison — normalized vs. denormalized queries

#### Lesson 5.4: `design_workshop.html` — ورشة التصميم
- **Full project:** Design a complete database from requirements
- **Scenario:** Egyptian e-commerce platform (like Jumia/Noon)
- **Steps:** Requirements → ER Diagram → Mapping → Normalization → Final Schema
- **Interactive:** Build the entire schema step-by-step with validation

---

### 🌊 UNIT 6: الـ Backend والـ ORM — Backend Integration
**Level:** Intermediate → Advanced | **Lessons:** 5 | **Color:** `#06B6D4` (Cyan)

> *"دلوقتي هنربط كل اللي اتعلمناه بـ Backend حقيقي — NestJS + Prisma + PostgreSQL"*

#### Lesson 6.1: `express_pg_basics.html` — Express.js + PostgreSQL
- **Concept:** Connecting a Node.js app to PostgreSQL
- **Content:** `pg` library, connection pools, parameterized queries
- **Project:** Simple REST API for a Student Management System
- **Security:** SQL Injection prevention — interactive demo showing the attack and the fix
- **Code lab:** Step-by-step with copyable code

#### Lesson 6.2: `prisma_intro.html` — مقدمة في Prisma ORM
- **Concept:** What is an ORM? Why Prisma?
- **Setup:** `npx prisma init`, `schema.prisma`, `.env`
- **Schema definition:** Models, fields, relations, attributes (`@id`, `@unique`, `@default`, `@relation`)
- **Prisma Client:** Auto-generated, type-safe database client
- **Prisma Studio:** Visual database browser (`npx prisma studio`)
- **Code lab:** Build a blog backend with Prisma

#### Lesson 6.3: `prisma_relations.html` — العلاقات في Prisma
- **One-to-One:** `@relation` with `@unique`
- **One-to-Many:** The most common pattern
- **Many-to-Many:** Implicit vs. explicit relations
- **Self-relations:** User following system
- **Visualization:** See the `schema.prisma` and the generated SQL side-by-side
- **Code lab:** Implement a social network data model

#### Lesson 6.4: `nestjs_prisma.html` — NestJS + Prisma
- **Why NestJS?** Modules, Dependency Injection, Decorators, scalability
- **PrismaService:** Creating a shared database service
- **CRUD Module:** Controller → Service → Prisma → PostgreSQL flow
- **DTOs and Validation:** `class-validator`, `class-transformer`
- **Code lab:** Build a full CRUD API for a Course Management System
- **Architecture diagram:** Interactive layer visualization

#### Lesson 6.5: `migrations_seeding.html` — Migrations و Seeding
- **Prisma Migrate:** `npx prisma migrate dev`, migration history
- **Schema evolution:** Adding columns, changing types, adding relations safely
- **Seeding:** `prisma/seed.ts` for populating development databases
- **Best practices:** Migration strategies for production
- **Interactive:** Timeline visualization of migration history

---

### 🔴 UNIT 7: المعاملات والتزامن — Transactions & Concurrency
**Level:** Advanced (Academic-Heavy) | **Lessons:** 4 | **Color:** `#EF4444` (Red)

> *"إزاي الـ Database بتتعامل مع آلاف الطلبات في نفس الوقت من غير ما الداتا تبوظ؟"*

> [!NOTE]
> This unit covers ACID properties, concurrency control, and recovery — core exam material at all Egyptian CS faculties. Maps directly to Elmasri & Navathe Chapters 20-22.

#### Lesson 7.1: `acid_transactions.html` — خصائص ACID
- **ACID:** Atomicity, Consistency, Isolation, Durability — explained with Egyptian bank transfer example
- **Visualization:** Animated bank transfer showing what happens when each property is violated
- **SQL Playground:** 
  ```sql
  BEGIN; UPDATE accounts SET balance = balance - 1000 WHERE id = 1; 
  -- What happens if the server crashes here?
  COMMIT;
  ```
- **Savepoints:** `SAVEPOINT`, `ROLLBACK TO`

#### Lesson 7.2: `concurrency_problems.html` — مشاكل التزامن
- **Problems:** Lost Update, Dirty Read, Non-Repeatable Read, Phantom Read
- **Visualization:** **Two-timeline animator** — see two transactions executing concurrently
- **Each problem:** Animated scenario showing exactly what goes wrong
- **Egyptian analogy:** "تخيل اتنين بيسحبوا من نفس الحساب في نفس الثانية" 💸

#### Lesson 7.3: `isolation_levels.html` — مستويات العزل
- **Levels:** Read Uncommitted → Read Committed → Repeatable Read → Serializable
- **PostgreSQL default:** Read Committed — why?
- **Visualization:** Matrix showing which problems each level prevents
- **SQL Playground:** Set isolation levels and observe behavior
- **Performance trade-offs:** Lock contention visualization

#### Lesson 7.4: `locking_recovery.html` — Locks و Recovery
- **Locking:** Shared locks, Exclusive locks, Two-Phase Locking (2PL)
- **Deadlocks:** Detection and prevention — animated deadlock scenario
- **Recovery:** Write-Ahead Logging (WAL), checkpoints, ARIES algorithm basics
- **Visualization:** Lock manager showing which transactions hold which locks
- **Academic:** Serialization graph, conflict serializability

---

### ⚡ UNIT 8: الأداء والفهرسة — Performance & Indexing
**Level:** Advanced | **Lessons:** 4 | **Color:** `#F59E0B` (Amber-Gold)

> *"الفرق بين query بتاخد 5 ثواني و query بتاخد 5 milliseconds هو الـ Indexing"*

#### Lesson 8.1: `explain_analyze.html` — قراءة خطة التنفيذ
- **`EXPLAIN ANALYZE`:** Understanding query execution plans
- **Visualization:** **Query plan tree visualizer** — see Seq Scan, Index Scan, Hash Join, etc.
- **Cost model:** Startup cost vs. total cost, rows estimation
- **SQL Playground:** Write queries and see their execution plans visualized
- **Practical:** "ليه الـ query دي بطيئة؟ خلينا نشوف"

#### Lesson 8.2: `indexing_deep_dive.html` — الفهرسة بالتفصيل
- **B-Tree index:** How it works internally — **animated B-Tree insertion and search**
- **Other types:** Hash index, GIN (for JSONB/arrays), GiST (for geometric/full-text), BRIN (for large sequential data)
- **When to index:** Selective columns, JOIN columns, WHERE clause columns
- **When NOT to index:** Small tables, frequently updated columns, low-cardinality columns
- **Visualization:** B-Tree growing as you insert data
- **Index scan vs. Seq scan:** Visual comparison with benchmarks

#### Lesson 8.3: `query_optimization.html` — تحسين الاستعلامات
- **Common anti-patterns:** `SELECT *`, functions in WHERE, implicit type conversion
- **Optimization techniques:** Covering indexes, partial indexes, expression indexes
- **`pg_stat_statements`:** Finding slow queries
- **Benchmarking:** Before vs. after optimization with real numbers
- **Interactive:** "Fix the slow query" challenges

#### Lesson 8.4: `partitioning_scaling.html` — التقسيم والتوسع
- **Table Partitioning:** Range, List, Hash partitioning in PostgreSQL
- **Connection Pooling:** PgBouncer, built-in NestJS pooling
- **Read Replicas:** Streaming replication basics
- **Visualization:** Data distribution across partitions
- **When to partition:** Table size thresholds, query patterns

---

### 🌐 UNIT 9: NoSQL وقواعد البيانات الحديثة — NoSQL & Modern Databases
**Level:** Advanced | **Lessons:** 4 | **Color:** `#14B8A6` (Teal)

> *"مش كل حاجة لازم تبقى في جدول — فيه أنواع تانية من قواعد البيانات عندها مميزات مختلفة"*

#### Lesson 9.1: `nosql_overview.html` — عالم الـ NoSQL
- **CAP Theorem:** Consistency, Availability, Partition Tolerance — you can only pick 2
- **Visualization:** Interactive CAP triangle — click each combination to see which databases fit
- **Types:** Document (MongoDB), Key-Value (Redis), Column-Family (Cassandra), Graph (Neo4j)
- **When SQL vs NoSQL:** Decision framework with real examples

#### Lesson 9.2: `mongodb_basics.html` — MongoDB الأساسيات
- **Documents and Collections:** JSON-like data model
- **CRUD:** `insertOne`, `find`, `updateOne`, `deleteOne`
- **Aggregation Pipeline:** `$match`, `$group`, `$project`, `$sort`
- **With NestJS:** Mongoose + NestJS integration basics
- **Interactive:** MongoDB playground with sample data

#### Lesson 9.3: `redis_caching.html` — Redis والتخزين المؤقت
- **Data structures:** Strings, Hashes, Lists, Sets, Sorted Sets
- **Caching patterns:** Cache-Aside, Write-Through, Write-Behind
- **With NestJS:** `@nestjs/cache-manager` + Redis
- **Use case:** Session management, rate limiting, real-time leaderboards
- **Visualization:** Cache hit/miss animation

#### Lesson 9.4: `choosing_database.html` — إزاي تختار الـ Database المناسبة
- **Decision matrix:** Interactive questionnaire → recommended database
- **Polyglot persistence:** Using multiple databases in one system
- **Real architectures:** How Uber, Netflix, Airbnb, and Careem use different databases together
- **Egyptian market:** What databases Egyptian companies use and why

---

### 🏆 UNIT 10: المشروع النهائي والمسار المهني — Capstone & Career
**Level:** All Levels | **Lessons:** 4 | **Color:** `#D946EF` (Fuchsia)

> *"كل اللي فات كان تحضير — دلوقتي وقت الشغل الحقيقي"*

#### Lesson 10.1: `capstone_ecommerce.html` — مشروع: منصة تجارة إلكترونية
- **Full project:** Design and build a complete e-commerce database
- **Requirements:** Users, Products, Categories, Orders, Payments, Reviews, Inventory
- **Stack:** NestJS + Prisma + PostgreSQL + Redis caching
- **Steps:** ER Design → Schema → Migrations → Seed Data → API → Optimization
- **Deliverable:** Working API with 15+ endpoints

#### Lesson 10.2: `capstone_analytics.html` — مشروع: لوحة تحليلات
- **Full project:** Build a student analytics dashboard
- **Content:** Complex aggregation queries, window functions, materialized views
- **Visualization:** Charts and graphs from database queries
- **Egyptian context:** "لوحة تحليلات لجامعة مصرية"

#### Lesson 10.3: `database_security.html` — أمان قواعد البيانات
- **Authentication:** `pg_hba.conf`, roles, privileges
- **Authorization:** `GRANT`, `REVOKE`, Row-Level Security (RLS)
- **Encryption:** Data at rest, data in transit, field-level encryption
- **SQL Injection deep-dive:** Advanced attack vectors and comprehensive prevention
- **Backup & Recovery:** `pg_dump`, `pg_restore`, Point-in-Time Recovery (PITR)
- **Interactive:** "Hack the database" challenge — find and fix SQL injection vulnerabilities

#### Lesson 10.4: `career_guide.html` — المسار المهني
- **Career paths:** Backend Developer, Database Administrator (DBA), Data Engineer, Data Analyst
- **Egyptian market:** Salary ranges, top companies hiring, required certifications
- **Skills matrix:** What to learn next after this course
- **Interview prep:** Top 30 database interview questions with detailed answers
- **Certifications:** Oracle OCP, AWS Database Specialty, PostgreSQL certification
- **Portfolio:** How to showcase your database projects

---

## 📁 Project Structure

```
database-mastery/
├── index.html                      # Main portal (10-unit grid)
├── README.md                       # Project documentation
├── css/
│   └── global-db.css               # Global design system
├── public/
│   ├── logo.svg                    # Database Mastery logo
│   └── og-image.png                # Social sharing image
│
├── Unit1/                          # عالم قواعد البيانات
│   ├── why_databases.html
│   ├── database_types.html
│   ├── database_architecture.html
│   ├── postgresql_setup.html
│   └── database_history.html
│
├── Unit2/                          # النموذج العلائقي و ER
│   ├── er_basics.html
│   ├── er_relationships.html
│   ├── eer_diagrams.html
│   ├── relational_model.html
│   └── er_to_relational.html
│
├── Unit3/                          # أساسيات SQL
│   ├── ddl_basics.html
│   ├── dml_crud.html
│   ├── aggregate_grouping.html
│   ├── joins_mastery.html
│   └── subqueries_sets.html
│
├── Unit4/                          # SQL المتقدم
│   ├── views_ctes.html
│   ├── window_functions.html
│   ├── advanced_types.html
│   └── functions_triggers.html
│
├── Unit5/                          # التصميم والتطبيع
│   ├── functional_dependencies.html
│   ├── normalization.html
│   ├── denormalization.html
│   └── design_workshop.html
│
├── Unit6/                          # Backend Integration
│   ├── express_pg_basics.html
│   ├── prisma_intro.html
│   ├── prisma_relations.html
│   ├── nestjs_prisma.html
│   └── migrations_seeding.html
│
├── Unit7/                          # المعاملات والتزامن
│   ├── acid_transactions.html
│   ├── concurrency_problems.html
│   ├── isolation_levels.html
│   └── locking_recovery.html
│
├── Unit8/                          # الأداء والفهرسة
│   ├── explain_analyze.html
│   ├── indexing_deep_dive.html
│   ├── query_optimization.html
│   └── partitioning_scaling.html
│
├── Unit9/                          # NoSQL الحديثة
│   ├── nosql_overview.html
│   ├── mongodb_basics.html
│   ├── redis_caching.html
│   └── choosing_database.html
│
├── Unit10/                         # المشروع النهائي
│   ├── capstone_ecommerce.html
│   ├── capstone_analytics.html
│   ├── database_security.html
│   └── career_guide.html
│
├── scripts/                        # El Daheeh-style video scripts
│   ├── unit1_scripts/
│   ├── unit2_scripts/
│   └── ...
│
├── tasks/                          # Hands-on practice exercises
│   ├── sql_challenges/
│   ├── design_challenges/
│   └── backend_projects/
│
├── reference/                      # Quick reference sheets
│   ├── sql_cheatsheet.html
│   ├── prisma_cheatsheet.html
│   └── postgresql_cheatsheet.html
│
├── slides/                         # Presentation slides
│   ├── unit1_slides.html
│   └── ...
│
├── notifications/                  # Smart notification system
│   └── README.md
│
├── backend/                        # NestJS project for Unit 6-10
│   ├── package.json
│   ├── tsconfig.json
│   ├── prisma/
│   │   ├── schema.prisma
│   │   ├── migrations/
│   │   └── seed.ts
│   └── src/
│       ├── app.module.ts
│       ├── main.ts
│       ├── prisma/
│       │   └── prisma.service.ts
│       ├── modules/
│       │   ├── students/
│       │   ├── courses/
│       │   ├── enrollments/
│       │   └── auth/
│       └── common/
│
└── sql-playground/                 # Embeddable SQL playground component
    ├── playground.js               # PGlite-based SQL executor  
    ├── playground.css              # Playground styling
    └── schemas/                    # Pre-loaded database schemas
        ├── university.sql
        ├── ecommerce.sql
        └── social_network.sql
```

---

## 🎨 Complete Design System & Styling Guide

> [!IMPORTANT]
> This section is the **definitive reference** for every visual decision in the project. Follow it exactly to achieve the same premium, glass-morphism dark-mode aesthetic as the algorithms project, with full RTL/bilingual support.

---

### 🎨 1. Color Palette

#### Unit Colors (Each unit gets a signature color for cards, accents, glows)
| Unit | Name | Primary Hex | Light Variant | Dark Variant | Glow `rgba` |
|------|------|-------------|--------------|-------------|-------------|
| 1 | Emerald | `#10B981` | `#34D399` | `#059669` | `rgba(16, 185, 129, 0.2)` |
| 2 | Blue | `#3B82F6` | `#60A5FA` | `#1D4ED8` | `rgba(59, 130, 246, 0.2)` |
| 3 | Amber | `#F59E0B` | `#FBBF24` | `#D97706` | `rgba(245, 158, 11, 0.2)` |
| 4 | Orange | `#F97316` | `#FB923C` | `#EA580C` | `rgba(249, 115, 22, 0.2)` |
| 5 | Purple | `#8B5CF6` | `#A78BFA` | `#6D28D9` | `rgba(139, 92, 246, 0.2)` |
| 6 | Cyan | `#06B6D4` | `#22D3EE` | `#0891B2` | `rgba(6, 182, 212, 0.2)` |
| 7 | Red | `#EF4444` | `#F87171` | `#DC2626` | `rgba(239, 68, 68, 0.2)` |
| 8 | Gold | `#EAB308` | `#FACC15` | `#CA8A04` | `rgba(234, 179, 8, 0.2)` |
| 9 | Teal | `#14B8A6` | `#2DD4BF` | `#0D9488` | `rgba(20, 184, 166, 0.2)` |
| 10 | Fuchsia | `#D946EF` | `#E879F9` | `#C026D3` | `rgba(217, 70, 239, 0.2)` |

#### Core Theme Colors
```css
/* Background layers (darkest → lightest) */
--bg-body:       #020617;   /* slate-950 — the void */
--bg-card:       #0F172A;   /* slate-900 — glass cards */
--bg-alt:        #1E293B;   /* slate-800 — inputs, code blocks */
--bg-hover:      rgba(255, 255, 255, 0.04);

/* Text hierarchy */
--text-primary:  #F1F5F9;   /* slate-100 — headings, important */
--text-body:     #E2E8F0;   /* slate-200 — body text */
--text-muted:    #94A3B8;   /* slate-400 — descriptions */
--text-faint:    #64748B;   /* slate-500 — timestamps, labels */
--text-ghost:    #475569;   /* slate-600 — disabled, footer */

/* Borders & dividers */
--border-subtle: rgba(255, 255, 255, 0.06);
--border-light:  rgba(255, 255, 255, 0.1);
--border-hover:  rgba(255, 255, 255, 0.15);
```

---

### ✍️ 2. Typography System

#### Font Stack (Three fonts, three purposes)
```html
<!-- Load in <head> of EVERY page -->
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&family=Inter:wght@400;500;600;700;800&family=Fira+Code:wght@400;500&display=swap" rel="stylesheet">
```

| Font | Purpose | Where Used |
|------|---------|-----------|
| **Cairo** (400-800) | Arabic text, Arabic headings, RTL blocks | All Arabic paragraphs, section titles, descriptions |
| **Inter** (400-800) | English text, English headings, UI elements | Nav items, stat numbers, lesson names, badges |
| **Fira Code** (400-500) | Code blocks, SQL queries, terminal output | SQL playground, code examples, inline `code` |

#### Type Scale
```css
/* Headings */
h1 { font-size: clamp(2.2rem, 5vw, 3.5rem); font-weight: 800; line-height: 1.2; }
h2 { font-size: clamp(1.6rem, 3vw, 2.5rem); font-weight: 700; }
h3 { font-size: 1.5rem; font-weight: 700; }
h4 { font-size: 1.2rem; font-weight: 600; }

/* Body text */
.body-text    { font-size: 1.1rem; line-height: 2.0; }   /* Arabic needs extra line-height */
.body-english { font-size: 1rem;   line-height: 1.7; }
.caption      { font-size: 0.85rem; line-height: 1.5; }
.code-text    { font-size: 0.92rem; line-height: 1.7; font-family: 'Fira Code'; }
```

#### Font Assignment Rule
```css
/* Arabic content containers */
.rtl-block, [dir="rtl"], .font-arabic {
    font-family: 'Cairo', sans-serif;
    line-height: 2.2;      /* Arabic script needs more vertical breathing room */
    letter-spacing: 0;
}

/* English content & UI */
body, .font-english, nav, .stat-number, .lesson-name {
    font-family: 'Inter', sans-serif;
}

/* Code everywhere */
code, pre, .code-box, .sql-editor, .font-mono {
    font-family: 'Fira Code', 'SF Mono', 'Consolas', monospace;
}
```

---

### 🔄 3. RTL / Bilingual System — THE CRITICAL SECTION

> [!CAUTION]
> This is the most important styling section. Getting RTL wrong makes the entire platform look broken. Follow these rules **exactly**.

#### Page-Level Direction Strategy

**Lesson pages are LTR by default** (because code, SQL, and technical content is LTR), with **Arabic blocks wrapped in RTL containers**:

```html
<!-- ✅ CORRECT: Page is LTR, Arabic blocks are RTL -->
<html lang="en" dir="ltr">
  <body>
    <!-- Nav, code, playground = naturally LTR -->
    
    <!-- Arabic explanation blocks get their own direction -->
    <div class="rtl-block">
      <h3 class="font-arabic">🔍 إيه هو البحث الثنائي؟</h3>
      <p>تخيل إنك عايز تدور على كلمة...</p>
    </div>
  </body>
</html>
```

```html
<!-- ✅ CORRECT: Portal page (index.html) is RTL because it's primarily Arabic -->
<html lang="ar" dir="rtl">
```

```html
<!-- ✅ CORRECT: Script pages are fully RTL -->
<html lang="ar" dir="rtl">
```

#### The RTL Block CSS (Core Utility)
```css
/* The single most important class in the project */
.rtl-block {
    direction: rtl;
    text-align: right;
    font-family: 'Cairo', sans-serif;
    line-height: 2.2;
}

/* When English text appears INSIDE an RTL block */
.rtl-block .english,
.rtl-block code,
.rtl-block .inline-code {
    direction: ltr;
    display: inline-block;        /* Prevents RTL reordering */
    font-family: 'Inter', sans-serif;
    unicode-bidi: embed;          /* Crucial for mixed-direction text */
}

/* Inline English terms in Arabic sentences */
.english {
    direction: ltr;
    display: inline-block;
    font-family: 'Inter', sans-serif;
    color: #93C5FD;               /* Light blue — makes English terms stand out */
    font-style: italic;
    font-weight: bold;
    unicode-bidi: embed;
}
```

#### Bilingual Heading Pattern
Every section has **both** an Arabic title and an English subtitle:
```html
<h2 class="text-4xl font-bold text-center mb-4">
    <i class="fa-solid fa-lightbulb text-yellow-500 mr-3"></i>
    الفكرة الأساسية
</h2>
<p class="text-center text-slate-400 mb-12">Understanding the Core Concept</p>
```

#### Mixed-Content Rules
| Scenario | How to Handle |
|----------|--------------|
| Arabic paragraph with English term | `<span class="english">Binary Search</span>` inside `.rtl-block` |
| Code block inside Arabic section | `<div class="code-box">` with `direction: ltr; text-align: left;` |
| Inline code in Arabic text | `<code class="inline-code bg-slate-800 px-2 py-0.5 rounded">SELECT</code>` |
| List with Arabic text | `<ul>` inside `.rtl-block` — bullets appear on the right |
| Table with mixed content | Table container is LTR, but Arabic cells get `text-align: right` |
| Nav links (Arabic) | Individual `<a>` tags, parent nav gets `direction: rtl` on portal page |

#### Border Direction for RTL
```css
/* In RTL, "left border" accents become "right border" accents */
.rtl-block .script-text    { border-right: 4px solid #06B6D4; border-left: none; }
.rtl-block .note            { border-right: 3px solid #FBBF24; border-left: none; }
.rtl-block .step-box        { border-right: 4px solid #06B6D4; border-left: none; }
.rtl-block .law-box         { border-right: 3px solid #3B82F6; border-left: none; }
.rtl-block .camera-cue      { border-right: 2px solid #EF4444; border-left: none; }

/* Code blocks are always LTR even inside RTL containers */
.code-box {
    direction: ltr;
    text-align: left;
    font-family: 'Fira Code', monospace;
    border-right: 3px solid #06B6D4;   /* Accent stays on right for visual consistency */
}
```

#### Arrow & Chevron Direction
```css
/* In RTL layout, navigation arrows flip */
[dir="rtl"] .lesson-arrow   { transform: rotate(180deg); }
[dir="rtl"] .back-arrow     { transform: rotate(180deg); }

/* Hover effects flip X direction too */
[dir="rtl"] .lesson-item:hover { transform: translateX(6px); }  /* was -6px in LTR */
```

---

### 🪟 4. Glass-Morphism Recipe (The Signature Look)

Every card in the platform uses this exact recipe:

```css
.glass-card {
    background: rgba(15, 23, 42, 0.7);      /* semi-transparent slate-900 */
    backdrop-filter: blur(12px);             /* the "glass" effect */
    -webkit-backdrop-filter: blur(12px);     /* Safari support */
    border: 1px solid rgba(255, 255, 255, 0.08);  /* thin white border */
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.22, 1, 0.36, 1);
}

.glass-card:hover {
    border-color: rgba(255, 255, 255, 0.12);
    transform: translateY(-4px);
    box-shadow: 0 20px 60px -15px var(--unit-glow-color);
}
```

#### Glass Variations
```css
/* Heavier glass for main content cards */
.glass-heavy {
    background: rgba(15, 23, 42, 0.85);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255, 255, 255, 0.1);
}

/* Lighter glass for nested elements */
.glass-light {
    background: rgba(255, 255, 255, 0.03);
    backdrop-filter: blur(8px);
    border: 1px solid rgba(255, 255, 255, 0.05);
}

/* Glass for nav/toolbar */
.glass-nav {
    background: rgba(2, 6, 23, 0.8);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid rgba(255, 255, 255, 0.06);
}
```

---

### ✨ 5. Animation & Micro-Interaction System

#### Scroll Reveal (AOS.js)
```html
<!-- Load AOS -->
<link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>AOS.init({ duration: 800, once: true, offset: 100 });</script>

<!-- Usage on elements -->
<div class="glass-card" data-aos="fade-up">...</div>
<div class="glass-card" data-aos="fade-right" data-aos-delay="200">...</div>
```

#### Aurora Glow Background (Portal Page)
```css
.aurora {
    position: absolute;
    border-radius: 50%;
    filter: blur(100px);
    opacity: 0;
    animation: auroraIn 2s ease forwards;
    pointer-events: none;
}
.aurora-1 {
    width: 500px; height: 500px;
    top: -10%; left: -5%;
    background: rgba(16, 185, 129, 0.12);  /* Emerald for DB theme */
    animation: auroraIn 2s ease forwards, auroraFloat1 20s ease-in-out infinite 2s;
}
.aurora-2 {
    width: 400px; height: 400px;
    bottom: 10%; right: -5%;
    background: rgba(6, 182, 212, 0.10);   /* Cyan accent */
}
```

#### Gradient Text Effect
```css
.text-gradient {
    background: linear-gradient(135deg, #10B981 0%, #06B6D4 40%, #3B82F6 70%, #8B5CF6 100%);
    background-size: 300% 100%;
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: gradientShift 8s ease infinite;
}
@keyframes gradientShift {
    0%, 100% { background-position: 0% 50%; }
    50%      { background-position: 100% 50%; }
}
```

#### Card Tilt Effect (On Hover)
```javascript
document.querySelectorAll('.unit-card').forEach(card => {
    card.addEventListener('mousemove', e => {
        const rect = card.getBoundingClientRect();
        const x = (e.clientX - rect.left) / rect.width - 0.5;
        const y = (e.clientY - rect.top) / rect.height - 0.5;
        card.style.transform = `translateY(-6px) perspective(800px) rotateX(${-y * 4}deg) rotateY(${x * 4}deg)`;
    });
    card.addEventListener('mouseleave', () => {
        card.style.transform = 'translateY(0)';
    });
});
```

#### Top-Glow Line on Cards (Hover)
```css
.unit-card::before {
    content: '';
    position: absolute;
    top: 0; left: 20%; right: 20%;
    height: 1px;
    border-radius: 1px;
    background: linear-gradient(90deg, transparent, var(--unit-color), transparent);
    opacity: 0;
    transition: opacity 0.4s ease;
}
.unit-card:hover::before { opacity: 1; }
```

#### Floating Particles Canvas
Reuse the same particle system from algorithms `index.html` but with database-themed hues:
```javascript
// Change particle hue to emerald/cyan instead of blue/purple
this.hue = Math.random() > 0.5 ? 160 : 190;  // emerald = 160, cyan = 190
```

#### Custom Scrollbar
```css
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb { background: rgba(255, 255, 255, 0.08); border-radius: 3px; }
::-webkit-scrollbar-thumb:hover { background: rgba(255, 255, 255, 0.15); }
```

---

### 🧩 6. Component Library (Reusable Patterns)

#### Unit Card (Portal Page)
```html
<div class="unit-card unit-3" id="unit-card-3">
    <div class="unit-header">
        <div class="unit-number">3</div>
        <div class="unit-info">
            <div class="unit-title">أساسيات SQL</div>
            <div class="unit-subtitle">SQL Fundamentals</div>
        </div>
    </div>
    <div class="lessons-list">
        <a href="Unit3/ddl_basics.html" class="lesson-item">
            <div class="lesson-icon"><i class="fas fa-table"></i></div>
            <div class="lesson-text">
                <div class="lesson-name">DDL Basics</div>
                <div class="lesson-desc">إنشاء الجداول — CREATE, ALTER, DROP</div>
            </div>
            <i class="fas fa-chevron-left lesson-arrow"></i>
        </a>
    </div>
</div>
```

#### Step Box (Explanations)
```html
<div class="step-box">
    <strong class="hl-cyan">① حدد المنطقة</strong>
    <br>حط الـ <code class="inline-code">WHERE</code> عشان تحدد الصفوف...
</div>
```

#### Note/Warning Boxes
```html
<!-- Note (Yellow) -->
<div class="note">ده بيشتغل بس لو الجدول فيه Primary Key</div>

<!-- Law/Rule Box (Blue) -->
<div class="law-box">
    <strong>القاعدة:</strong>
    <br>كل جدول لازم يكون فيه Primary Key واحد على الأقل.
</div>

<!-- Warning Box (Red) -->
<div class="warning-box">
    <strong>⚠️ تحذير:</strong>
    <br>DROP TABLE بيمسح الجدول نهائياً! مفيش Undo!
</div>
```

#### Code Block with Arabic Label
```html
<div class="code-box">
-- إنشاء جدول الطلاب
CREATE TABLE students (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(255) UNIQUE,
    gpa NUMERIC(3,2) CHECK (gpa >= 0 AND gpa <= 4)
);</div>
```
```css
.code-box {
    direction: ltr;
    text-align: left;
    font-family: 'Fira Code', monospace;
    font-size: 0.92rem;
    color: #A5F3FC;
    background: rgba(0, 0, 0, 0.45);
    padding: 1rem 1.2rem;
    border-radius: 8px;
    border-right: 3px solid #06B6D4;
    line-height: 1.7;
    overflow-x: auto;
    white-space: pre-wrap;
}
/* Auto-label "💻 الكود:" above code blocks */
.code-box::before {
    content: "💻 الكود: ";
    font-weight: bold;
    color: #22D3EE;
    display: block;
    direction: rtl;
    text-align: right;
    font-family: 'Cairo', sans-serif;
    margin-bottom: 0.5rem;
    font-size: 0.9rem;
}
```

#### Colored Text Helpers
```css
.highlight   { color: #34D399; font-weight: 700; }  /* green success */
.hl-blue     { color: #60A5FA; font-weight: 700; }  /* blue info */
.hl-amber    { color: #FBBF24; font-weight: 700; }  /* yellow warning */
.hl-red      { color: #F87171; font-weight: 700; }  /* red danger */
.hl-cyan     { color: #22D3EE; font-weight: 700; }  /* cyan accent */
.hl-purple   { color: #A78BFA; font-weight: 700; }  /* purple special */
```

#### Comparison Table
```css
.comparison-table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.9rem;
}
.comparison-table th {
    background: rgba(6, 182, 212, 0.1);
    color: #22D3EE;
    padding: 0.5rem;
    text-align: right;              /* RTL-aware */
    border: 1px solid rgba(255, 255, 255, 0.06);
}
.comparison-table td {
    padding: 0.5rem;
    border: 1px solid rgba(255, 255, 255, 0.06);
    color: #CBD5E1;
}
.comparison-table tr:hover {
    background: rgba(255, 255, 255, 0.02);
}
```

---

### 🎬 7. El Daheeh (الدحيح) Writing Style Guide

> [!IMPORTANT]
> **This is the soul of the platform.** Every Arabic explanation must feel like a conversation with a brilliant, funny friend who happens to be a database expert — NOT like reading a textbook. Read the existing algorithm scripts (e.g., `scripts/binary_search_script.html`) to internalize this style.

#### Core Principles of the El Daheeh Style

**1. Start with a HOOK — بداية تخطف الانتباه**
Never start with a definition. Start with a story, challenge, or question:
```
❌ "قاعدة البيانات هي مجموعة منظمة من البيانات..."
✅ "تخيل إنك مسؤول عن تسجيل 50,000 طالب في جامعة القاهرة. عندك Excel فيه كل الداتا. 
   فجأة حد قالك: 'ابعتلي أرقام تليفونات كل طلاب هندسة اللي معنديهم رقم قومي.' 
   ... كويس. حظ سعيد مع VLOOKUP. 😅"
```

**2. Egyptian Street Arabic — مصري شوارعي حقيقي**
Use real Egyptian dialect, not formal Arabic (فصحى):

| ❌ Formal (Academic) | ✅ Egyptian (Daheeh) |
|---------------------|---------------------|
| يجب عليك أن تقوم بإنشاء | لازم تعمل |
| نستطيع أن نلاحظ أن | هتلاقي إن |
| يتم استخدام هذا الأمر في | الأمر ده بنستخدمه عشان |
| وفقاً للبيانات المتاحة | بناءً على الداتا اللي عندنا |
| دعونا نستعرض | يلا نشوف |
| هل تعلم أن | تعرف إن |
| يعتبر هذا من أهم | ده من أهم |
| قم بتنفيذ الأمر التالي | اكتب الأمر ده |

**3. English Technical Terms Stay English** — المصطلحات الإنجليزية تفضل إنجليزي
Never translate technical terms. Wrap them in `<span class="english">`:
```
❌ "أنشئ جدولاً جديداً باستخدام لغة الاستعلام الهيكلية"
✅ "اعمل <span class='english'>Table</span> جديد بالـ <span class='english'>SQL</span>"
```

Common terms that MUST stay in English:
`Database`, `Table`, `Primary Key`, `Foreign Key`, `SELECT`, `INSERT`, `JOIN`, `Index`, `Query`, `ORM`, `Prisma`, `NestJS`, `PostgreSQL`, `Transaction`, `ACID`, `Normalization`, `API`, `CRUD`, `Schema`, `Migration`, `ER Diagram`

**4. Build Mental Models with Analogies — التشبيهات**
Every concept needs a real-world Egyptian analogy BEFORE the technical definition:

```
💡 PRIMARY KEY:
"تخيل إنك في الجيش. كل مجند ليه رقم عسكري مميز. 
 مفيش اتنين ليهم نفس الرقم. ولازم كلهم يكون عندهم واحد. 
 ده بالظبط الـ Primary Key — رقم مميز لكل صف في الجدول. 
 مينفعش يتكرر. ومينفعش يبقى فاضي."

💡 FOREIGN KEY:
"الرقم العسكري ده لو كتبته في جدول تاني — 
 مثلاً جدول 'المهمات' — ده بقى Foreign Key. 
 بيقول: 'أنا مش المجند نفسه... أنا بس بشاور عليه.'"

💡 JOIN:
"تخيل عندك ورقة فيها أسماء الطلاب، وورقة تانية فيها درجاتهم. 
 عايز تحط الاتنين جنب بعض عشان تشوف 'مين جاب كام.' 
 ده الـ JOIN. بتجمع جدولين مع بعض بناءً على حاجة مشتركة بينهم."
```

**5. Progressive Reveal — كشف تدريجي**
Don't dump everything at once. Build suspense:
```
"طيب... فيه مشكلة."
(beat)
"تخيل اتنين بيسحبوا من نفس الحساب في نفس الثانية."
(beat) 
"واحد بيسحب 500 والتاني بيسحب 300. الرصيد 1000."
(beat)
"الاتنين قروا الرصيد: 1000. الاتنين خصموا: 500 + 300."
(beat)
"الرصيد المفروض: 200. الرصيد الفعلي: 500. 😱"
(beat)
"ده اسمه... Lost Update Problem."
```

**6. Celebration at Key Moments — احتفال**
When the student achieves something, CELEBRATE:
```
🎉 "لقيناه!! SELECT اشتغل!! أول query في حياتك!!"
✅ "كده الجدول بتاعك في 3NF. مبروووك! 🎉🎉🎉"
🏆 "خلصت Unit 3!! بقيت تتكلم SQL زي الماء! 💪"
```

**7. Camera/VFX/SFX Cues** (For script pages only)
These go in the `scripts/` directory for video production:
```html
<span class="camera-cue">🎥 [Close-up على الوش، بتبص للكاميرا بتحدي]</span>
<span class="vfx-cue">✨ [VFX: الجدول بيتقسم لجدولين — أنيميشن Normalization]</span>
<span class="sfx-cue">🔊 [SFX: صوت BOOM خفيف]</span>
```

#### Script Page Styling (CSS for `scripts/` pages)
```css
body {
    font-family: 'Cairo', sans-serif;
    background: linear-gradient(135deg, #0a0a1a, #0f1a2e, #0a1628);
    direction: rtl;
    color: #e0e0e0;
}
.script-text {
    font-size: 1.12rem;
    line-height: 2.2;
    color: #f0f4f8;
    background: rgba(0, 0, 0, 0.25);
    padding: 1.2rem 1.5rem;
    border-radius: 10px;
    border-right: 4px solid #06B6D4;
}
.camera-cue {
    font-size: 0.85rem;
    color: #FCA5A5;
    display: block;
    font-weight: bold;
    background: rgba(239, 68, 68, 0.1);
    padding: 0.3rem 0.5rem;
    border-radius: 4px;
    border-right: 2px solid #EF4444;
}
.vfx-cue {
    font-size: 0.85rem;
    color: #93C5FD;
    display: block;
    font-weight: bold;
    background: rgba(59, 130, 246, 0.1);
    padding: 0.3rem 0.5rem;
    border-radius: 4px;
    border-right: 2px solid #3B82F6;
}
.sfx-cue {
    font-size: 0.85rem;
    color: #D8B4FE;
    display: block;
    font-weight: bold;
    background: rgba(168, 85, 247, 0.1);
    padding: 0.3rem 0.5rem;
    border-radius: 4px;
    border-right: 2px solid #A855F7;
}
```

#### Sample El Daheeh Database Text (Reference)
```
🎬 Topic: Why do we need Foreign Keys?

"طيب سؤال: إنت عملت جدول الطلاب. عملت جدول الأقسام. تمام.

بس... لو طالب كتبت في خانة 'القسم' بتاعه: 'قسم الفضاء الخارجي.' 
ده قسم مش موجود أصلاً!

يعني الداتا بتاعتك بقت... كذب. 🤥 بيانات مالهاش معنى.

وده بالظبط المشكلة اللي الـ Foreign Key بيحلها. 
بيقول للـ Database: 'يا سيدي، القيمة دي — لازم تكون موجودة في الجدول التاني. 
لو حد حاول يحط قيمة مش موجودة هناك — ارفض. اضربه بالخطأ. 
ERROR: insert or update violates foreign key constraint.'

في الحقيقة، ده زي ما تبقى بتسجل في الجامعة وتقول 'أنا عايز أسجل في كلية هوجوورتس.' 
النظام هيرد عليك: 'مفيش كلية بالاسم ده. روح ابعد. 🧙‍♂️'

وده اسمه: Referential Integrity. يعني 'سلامة المراجع.' 
كل Reference تعمله، لازم يكون صحيح ومتحقق منه."
```

---

### 📐 8. Lesson Page Template (Complete HTML Skeleton)

Every lesson page follows this architecture:

```html
<!DOCTYPE html>
<html lang="en" class="scroll-smooth" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JOIN Mastery | إتقان الـ Joins</title>
    <meta name="description" content="تعلم كل أنواع الـ Joins في SQL بطريقة تفاعلية">
    
    <!-- Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&family=Inter:wght@400;500;600;700;800&family=Fira+Code:wght@400;500&display=swap" rel="stylesheet">
    <!-- Icons -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <!-- AOS Animations -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <!-- TailwindCSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        neon: { green: '#10B981', blue: '#3B82F6', amber: '#F59E0B', cyan: '#06B6D4' },
                        dark: { bg: '#020617', card: '#0F172A', border: '#1E293B' }
                    },
                    fontFamily: { sans: ['Inter'], arabic: ['Cairo'], mono: ['Fira Code'] }
                }
            }
        }
    </script>
    <style>
        body { background: #020617; color: #E2E8F0; overflow-x: hidden; }
        .glass-card { background: rgba(15, 23, 42, 0.7); backdrop-filter: blur(12px); border: 1px solid rgba(255, 255, 255, 0.08); }
        .text-gradient { background: linear-gradient(135deg, #F59E0B, #F97316); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; }
        .rtl-block { direction: rtl; text-align: right; font-family: 'Cairo', sans-serif; line-height: 2.2; }
        .english { direction: ltr; display: inline-block; font-family: 'Inter', sans-serif; color: #93C5FD; font-style: italic; font-weight: bold; unicode-bidi: embed; }
        /* ... (all component CSS from Section 6 above) ... */
    </style>
</head>
<body>
    <!-- 1. FIXED NAVBAR -->
    <nav class="fixed top-0 w-full z-50 glass-card border-b-0">
        <div class="container mx-auto px-6 h-16 flex items-center justify-between">
            <a href="../index.html" class="flex items-center gap-3">
                <div class="w-8 h-8 rounded bg-gradient-to-br from-amber-500 to-orange-500 flex items-center justify-center text-white font-bold">
                    <i class="fas fa-arrow-left text-sm"></i>
                </div>
                <span class="font-bold text-lg">JOIN<span class="text-amber-500">Mastery</span></span>
            </a>
            <div class="hidden md:flex gap-8 text-sm font-medium text-slate-400">
                <a href="#concept" class="hover:text-amber-400 transition">المفهوم</a>
                <a href="#detailed" class="hover:text-amber-400 transition">الشرح التفصيلي</a>
                <a href="#playground" class="hover:text-amber-400 transition">التجربة</a>
                <a href="#code" class="hover:text-amber-400 transition">الكود</a>
            </div>
        </div>
    </nav>

    <!-- 2. HERO SECTION -->
    <header class="relative pt-32 pb-20 px-6 overflow-hidden">
        <div class="absolute top-0 right-0 w-[500px] h-[500px] bg-amber-500/10 rounded-full blur-[128px]"></div>
        <div class="container mx-auto text-center relative z-10" data-aos="fade-up">
            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-slate-800/50 border border-slate-700 text-xs font-mono text-amber-400 mb-6">
                <span class="w-2 h-2 rounded-full bg-amber-500 animate-pulse"></span>
                UNIT 3 • أساسيات SQL
            </div>
            <h1 class="text-5xl md:text-7xl font-black mb-6 tracking-tight">
                <span class="text-gradient">JOIN</span> Mastery
            </h1>
            <h2 class="text-3xl font-bold text-slate-400 font-arabic mb-8">إتقان الـ Joins</h2>
            <p class="text-lg text-slate-400 max-w-2xl mx-auto leading-relaxed">
                The most important SQL skill — connecting tables together.
            </p>
        </div>
    </header>

    <!-- 3. المفهوم (Concept) - RTL Arabic Block -->
    <section id="concept" class="py-20 px-6 bg-slate-900/30">
        <div class="container mx-auto max-w-5xl">
            <h2 class="text-4xl font-bold text-center mb-4">
                <i class="fa-solid fa-lightbulb text-yellow-500 mr-3"></i>
                الفكرة الأساسية
            </h2>
            <p class="text-center text-slate-400 mb-12">Understanding the Core Concept</p>
            
            <div class="glass-card p-8 rounded-2xl" data-aos="fade-up">
                <div class="rtl-block">
                    <h3 class="text-2xl font-bold text-amber-400 mb-6">
                        🔗 إيه هو الـ <span class="english">JOIN</span>؟
                    </h3>
                    <div class="space-y-6 text-lg">
                        <p class="text-slate-300">
                            تخيل عندك ورقتين. ورقة فيها أسماء الطلاب، وورقة تانية فيها درجاتهم.
                            عايز تحطهم جنب بعض عشان تشوف <span class="hl-amber">"مين جاب كام."</span>
                        </p>
                        <!-- ... more El Daheeh style content ... -->
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. INTERACTIVE SQL PLAYGROUND -->
    <section id="playground" class="py-20 px-6">
        <!-- SQL Playground component embedded here -->
    </section>

    <!-- 5. CODE IMPLEMENTATION -->
    <section id="code" class="py-20 px-6 bg-black/20">
        <!-- Side-by-side: Code (LTR) | Arabic explanation (RTL) -->
    </section>

    <!-- 6. MINI-PROJECT -->
    <section class="py-20 px-6">
        <!-- Hands-on exercise -->
    </section>

    <!-- 7. FOOTER -->
    <footer class="py-12 text-center text-slate-600 bg-black/40 text-sm">
        <p>Database Mastery — Unit 3: SQL Fundamentals</p>
        <p class="font-arabic mt-1">إتقان قواعد البيانات</p>
    </footer>

    <script>AOS.init({ duration: 800, once: true, offset: 100 });</script>
</body>
</html>
```

---

### 📱 9. Responsive Design Breakpoints

```css
/* Desktop: 5×2 unit grid */
@media (min-width: 1200px) {
    .units-container { grid-template-columns: repeat(5, 1fr); }
}

/* Tablet: 2 or 3 columns */
@media (max-width: 1199px) and (min-width: 768px) {
    .units-container { grid-template-columns: repeat(2, 1fr); }
    h1 { font-size: 2.2rem; }
}

/* Mobile: single column */
@media (max-width: 767px) {
    .units-container { grid-template-columns: 1fr; }
    h1 { font-size: 1.8rem; }
    .rtl-block { font-size: 1rem; line-height: 2; }
    .glass-card { padding: 16px; }
    .code-box { font-size: 0.8rem; padding: 0.8rem; }
}
```

### Portal Page Design
- Same dark theme with aurora glow effects (`#07070d` background)
- 10 unit cards in a responsive grid (5×2 on desktop, 2×5 on tablet, 1×10 on mobile)
- Particle canvas with database-themed floating icons (tables, keys, SQL symbols)
- Animated gradient title: "Database Mastery — إتقان قواعد البيانات"
- Progress tracking bar showing completed lessons

---

## 🔧 Key Interactive Components to Build

### 1. SQL Playground (`sql-playground/`)
- **Engine:** PGlite (WebAssembly PostgreSQL) for true PostgreSQL compatibility in-browser
- **Features:**
  - Multi-tab query editor with syntax highlighting
  - Results table with sorting and pagination
  - Schema explorer sidebar showing tables, columns, relationships
  - Pre-loaded sample databases (university, e-commerce, social network)
  - Exercise mode with auto-grading
  - Query history
- **Design:** Glass-morphism card with terminal-style editor

### 2. ER Diagram Builder
- **Canvas-based** interactive builder
- **Drag-and-drop** entities, attributes, relationships
- **Auto-layout** algorithm for clean diagrams
- **Export:** Generate SQL `CREATE TABLE` statements from the diagram
- **Import:** Generate ER diagram from existing SQL schema

### 3. Normalization Visualizer
- **Input:** A table with sample data and FDs
- **Output:** Step-by-step decomposition into normal forms
- **Animation:** Watch tables split and restructure
- **Verification:** Check if decomposition is lossless and dependency-preserving

### 4. Query Plan Visualizer
- **Input:** EXPLAIN ANALYZE output (JSON format)
- **Output:** Interactive tree diagram
- **Features:** Color-coded nodes (green = fast, red = slow), cost tooltips, row count comparison

### 5. Transaction Timeline Animator
- **Input:** Two concurrent transactions
- **Output:** Animated timeline showing read/write operations, locks, conflicts
- **Modes:** Show different isolation levels and their effects

---

## 📐 Alignment with Egyptian University Curricula

### Mapping to Elmasri & Navathe (Primary Textbook in Egypt)
| Textbook Chapter | Platform Unit |
|-----------------|---------------|
| Ch 1-2: Intro & Concepts | Unit 1 |
| Ch 3-4: ER Model | Unit 2 (2.1-2.3) |
| Ch 5: Relational Model | Unit 2 (2.4) |
| Ch 7-8: ER-to-Relational Mapping | Unit 2 (2.5) |
| Ch 6: SQL Basics | Unit 3 |
| Ch 9: Advanced SQL | Unit 4 |
| Ch 14-15: FDs & Normalization | Unit 5 |
| Ch 16-17: Physical Design & Indexing | Unit 8 |
| Ch 20-22: Transactions & Recovery | Unit 7 |
| Ch 24-25: NoSQL & Big Data | Unit 9 |

### FCIS Ain Shams — Database Course (CIS280) Coverage ✅
### FCAI Cairo University — DBMS Course Coverage ✅
### FCDS Alexandria University — Database Course Coverage ✅
### GUC — Database Systems Course Coverage ✅

---

## 🚀 Implementation Order

> [!TIP]
> Build in this order to have a usable platform as early as possible:

| Phase | What to Build | Why First |
|-------|--------------|-----------|
| **Phase 1** | `index.html` (portal) + `css/global-db.css` + SQL Playground component | Foundation — everything links from here |
| **Phase 2** | Unit 1 (5 lessons) | Onboarding — every student starts here |
| **Phase 3** | Unit 3 (5 lessons) | SQL is the most practical skill to learn early |
| **Phase 4** | Unit 2 (5 lessons) | ER/Relational model — academic requirement |
| **Phase 5** | Unit 5 (4 lessons) | Normalization — exam-critical |
| **Phase 6** | Unit 4 (4 lessons) | Advanced SQL — levels up career-track students |
| **Phase 7** | Unit 6 (5 lessons) + backend/ setup | Backend integration — the bridge to real projects |
| **Phase 8** | Unit 7 (4 lessons) | Transactions — academic requirement |
| **Phase 9** | Unit 8 (4 lessons) | Performance — advanced career skill |
| **Phase 10** | Unit 9 (4 lessons) | NoSQL — modern industry requirement |
| **Phase 11** | Unit 10 (4 lessons) | Capstone — pulls everything together |
| **Phase 12** | Scripts, tasks, reference sheets | Supporting materials |

---

## 📊 Total Scope

| Metric | Count |
|--------|-------|
| **Total Units** | 10 |
| **Total Lessons** | 44 |
| **Interactive Visualizations** | 44+ |
| **SQL Playground Exercises** | 100+ |
| **Backend Projects** | 5 |
| **Quick Reference Sheets** | 3 |
| **Design Challenges** | 10 |
| **Sample Databases** | 3 |

---

## ✅ Verification Plan

### Automated Tests
- All HTML pages validate (W3C validator)
- SQL Playground executes queries correctly against PGlite
- All navigation links work (no broken links)
- Responsive design tested at 320px, 768px, 1024px, 1440px

### Manual Verification
- Each lesson's Arabic content reviewed for accuracy and natural Egyptian dialect
- SQL exercises tested with correct and incorrect answers
- Backend project builds and runs with `npm run dev`
- Prisma migrations apply cleanly to a fresh PostgreSQL instance
- All visualizations are interactive and functional

### Browser Testing
- Open each lesson page in browser
- Verify SQL Playground functionality
- Verify interactive ER diagram builder
- Test all animations and transitions
- Verify bilingual content renders correctly (RTL Arabic + LTR English)

---

> [!IMPORTANT]
> ## Open Questions for You
> 
> 1. **Project location:** Should I create this as a new directory alongside your algorithms project (e.g., `d:\work\projects\database-mastery\`)? Or do you have a preferred location?
> 
> 2. **Language balance:** Your algorithms project mixes Arabic and English. Should this project follow the exact same balance, or would you like more/less Arabic?
> 
> 3. **Backend project:** Should the NestJS backend be a fully working project that students clone and build on, or should it be code snippets within the HTML lessons only?
> 
> 4. **SQL Playground engine:** PGlite gives real PostgreSQL in the browser (heavier, ~5MB) vs. sql.js which is SQLite (lighter, ~1MB but not PostgreSQL-compatible). Which do you prefer?
> 
> 5. **Should I start building now**, beginning with Phase 1 (portal + design system + SQL playground)?
