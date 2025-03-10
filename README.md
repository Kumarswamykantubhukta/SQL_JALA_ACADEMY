# SQL_JALA_ACADEMY

# README: SQL Queries for Sales Database

## Overview
This document contains SQL queries related to a sales database consisting of three tables: **Salespeople**, **Customers (Cust)**, and **Orders**. The queries address various business requirements such as finding relationships between salespeople and customers, calculating averages, and extracting specific data.

## Database Structure
The database consists of the following tables:

### Salespeople Table
| SNUM  | SNAME   | CITY      | COMM |
|-------|--------|-----------|------|
| 1001  | Peel   | London    | 0.12 |
| 1002  | Serres | San Jose  | 0.13 |
| 1004  | Motika | London    | 0.11 |
| 1007  | Rafkin | Barcelona | 0.15 |
| 1003  | Axelrod| New York  | 0.10 |

### Customers (Cust) Table
| CNUM  | CNAME   | CITY    | RATING | SNUM  |
|-------|--------|---------|--------|------|
| 2001  | Hoffman| London  | 100    | 1001 |
| 2002  | Giovanne| Rome    | 200    | 1003 |
| 2003  | Liu    | San Jose| 300    | 1002 |
| 2004  | Grass  | Brelin  | 100    | 1002 |
| 2006  | Clemens| London  | 300    | 1007 |
| 2007  | Pereira| Rome    | 100    | 1004 |

### Orders Table
| ONUM  | AMT    | ODATE       | CNUM  | SNUM  |
|-------|--------|------------|-------|------|
| 3001  | 18.69  | 03-OCT-94  | 2008  | 1007 |
| 3003  | 767.19 | 03-OCT-94  | 2001  | 1001 |
| 3002  | 1900.10| 03-OCT-94  | 2007  | 1004 |
| 3005  | 5160.45| 03-OCT-94  | 2003  | 1002 |
| 3006  | 1098.16| 04-OCT-94  | 2008  | 1007 |
| 3009  | 1713.23| 04-OCT-94  | 2002  | 1003 |
| 3007  | 75.75  | 05-OCT-94  | 2004  | 1002 |
| 3008  | 4723.00| 05-OCT-94  | 2006  | 1001 |
| 3010  | 1309.95| 06-OCT-94  | 2004  | 1002 |
| 3011  | 9891.88| 06-OCT-94  | 2006  | 1001 |

## SQL Queries

1. **Pairs of salespeople living in the same city**
2. **Pairs of orders by a given customer**
3. **Customers with the same rating as Hoffman**
4. **Orders associated with salesperson Motika**
5. **Orders credited to the same salesperson as Hoffman**
6. **Orders greater than the average for Oct 4**
7. **Average commission of salespeople in London**
8. **Orders attributed to salespeople serving customers in London**
9. **Commissions of salespeople serving customers in London**
10. **Customers with CNUM greater than SNUM of Serres + 1000**
11. **Count customers with rating above San Jose's average**

Each of these queries is included in the provided SQL script file. This script is designed to help with analytical queries related to the sales database.

## Usage
- Ensure that the database structure matches the provided tables.
- Run the queries in an SQL-compatible environment such as MySQL, PostgreSQL, or Oracle.
- Modify the queries as needed to adapt to specific requirements.

## Notes
- Ensure that the data types and constraints align with your SQL implementation.
- The queries assume that data integrity is maintained within the database.
- Some queries involve subqueries and JOIN operations to retrieve meaningful insights.



