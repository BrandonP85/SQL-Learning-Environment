# SQL-Learning-Environment
A collection of commits to act as a portfolio for my progress learning SQL

## Purpose

I work in escalations for a cloud-based healthcare SaaS platform, where I investigate complex issues, validate bug fixes in live environments, and hand findings to development. SQL is the natural next tool for that work. This repo documents how I'm building that skill, one commit at a time, by applying it to realistic support investigations instead of generic textbook exercises.

## Goals

- Build fluency in the SQL used for troubleshooting and root cause analysis
- Practice verifying data integrity before and after a bug fix
- Develop safe, read-only investigation habits
- Document my reasoning, not just my queries, the same way I document escalations

## The Environment

- **Database:** [PostgreSQL]
- **Data:** an entirely fictional SaaS schema (customers, users, tickets, appointments, audit log). All data is invented. No real customer, company, or patient information is used here.
- **Intentional messiness:** the seed data includes duplicates, orphaned records, reopened tickets, and inconsistent timestamps, because real investigations rarely start with clean data.

## Repository Structure

- `schema.sql`: table definitions
- `seed_data.sql`: fictional sample data
- `scenarios/`: one file per investigation, each with the question, the query, the result, and what it would tell me in a real escalation
- `notes/`: lessons learned and mistakes worth remembering

## How to Run

1. [PostgreSQL]
2. Create the database: `[command]`
3. Load `schema.sql`, then `seed_data.sql`
4. Open any file in `scenarios/` and run the queries

## Skills Roadmap

- [ ] SELECT, filtering, sorting
- [ ] JOINs across related tables
- [ ] GROUP BY, HAVING, and aggregates
- [ ] Subqueries and CTEs
- [ ] Date and time handling
- [ ] Finding duplicates and orphaned records
- [ ] Before/after validation of a data fix
- [ ] Query performance basics (indexes, EXPLAIN)

## Approach

Every scenario follows the same pattern: state the support question, write the query, record the result, then explain what it means and what I'd do next. Investigations are read-only (SELECT) by default. Any query that changes data is documented with how I'd verify it first.

## Status

Work in progress. Updated regularly. Scenarios are added as I complete them.

## About

Built by Brandon Parker as part of my transition into technical support engineering and software quality roles. See also my [QA Learning Lab](https://github.com/BrandonP85/qa-learning-lab).
