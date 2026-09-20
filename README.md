# Library Management System – SQL Server

## Project Overview

The **Library Management System** is a SQL Server database project designed to manage and analyze library operations such as books, members, employees, branches, book issues, and book returns.

The project demonstrates practical SQL skills including **database creation, table design, primary and foreign keys, data loading from CSV files, CRUD operations, joins, aggregation, GROUP BY, HAVING, CTAS/SELECT INTO, date functions, and subqueries/conditional filtering**.

## Objectives

* Design a relational database for a library management system.
* Manage books, members, employees, branches, issued books, and returned books.
* Establish relationships between different tables using primary and foreign keys.
* Import real-world-style CSV data into SQL Server.
* Perform business-oriented analysis using SQL queries.
* Identify issued and unreturned books.
* Analyze book issuance and rental income by category.
* Generate summary tables for reporting and analysis.

## Database Tables

The project contains the following tables:

* **Branch** – Stores library branch and manager information.
* **Employees** – Stores employee details and their assigned branch.
* **Books** – Stores book information including category, rental price, author, publisher, and availability status.
* **Members** – Stores library member information and registration dates.
* **Issued_Stauts** – Records book issue transactions.
* **Return_Status** – Records returned book transactions.

## Key SQL Concepts Used

* Database Creation and Management
* Table Creation
* Primary Keys
* Foreign Keys
* CRUD Operations
* BULK INSERT
* CSV Data Import
* INNER JOIN
* LEFT JOIN
* GROUP BY
* HAVING
* COUNT()
* SUM()
* ORDER BY
* WHERE Filtering
* DATEADD()
* GETDATE()
* SELECT INTO / CTAS-style table creation
* Self-Join
* NULL Handling
* Relational Database Design

## Key Analysis Performed

### 1. Book Management

Added new book records and created a separate table containing books with rental prices above $6.

### 2. Member Management

Updated member information, inserted new members, and identified members who registered within the last 180 days.

### 3. Issue Analysis

Analyzed books issued by specific employees and identified members who issued more than one book.

### 4. Category Analysis

Calculated the number of books issued and total rental income generated for each book category.

### 5. Employee and Branch Analysis

Used joins to display employees along with their respective managers and branches.

### 6. Return Analysis

Identified books that have been issued but have not yet been returned by comparing the `Issued_Stauts` and `Return_Status` tables.

## Project Workflow

```text
CSV Files
    ↓
SQL Server Database
    ↓
Tables & Relationships
    ↓
Data Import using BULK INSERT
    ↓
Data Validation
    ↓
SQL Analysis
    ↓
Business Insights
```

## Sample Business Questions

The project answers questions such as:

* Which books have been issued by a particular employee?
* Which members have issued more than one book?
* How many books are issued in each category?
* What is the total rental income by category?
* Which employees work under which branch managers?
* Which books have not yet been returned?
* Which books have a rental price above $6?
* Which members registered within the last 180 days?

## Tools & Technologies

**Database:** Microsoft SQL Server
**Language:** T-SQL
**Data Source:** CSV files
**Tool:** SQL Server Management Studio (SSMS)
**Version Control:** Git & GitHub

## Repository Contents

```text
Library-Management-System/
│
├── README.md
│
├── SQL/
│   └── Library_Management_System.sql
│
├── Data/
│   ├── branch.csv
│   ├── books.csv
│   ├── employees.csv
│   ├── issued_status.csv
│   ├── members.csv
│   └── return_status.csv
│
└── Screenshots/
    └── query_results/
```

## Skills Demonstrated

**SQL Server | T-SQL | Database Design | Data Import | Data Cleaning | Joins | Aggregations | Business Analysis | Relational Database | Data Analysis | GitHub**
