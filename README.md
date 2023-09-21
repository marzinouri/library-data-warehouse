# Library datawarehouse

This repository contains all the resources related to our operational database and datawarehouse for managing library-related data.

## Overview

Our datawarehouse is designed to efficiently store and analyze data from various sources in the library system. It includes an operational database with tables categorically organized and three data marts: Financial, Cultural, and Lending.

## Operational Database

### Categories and Sample Tables

- **Book Related Tables**:
  - `book`: Information about books.
  - `author`: Details of book authors.
  - `translator`: Information about book translators.
  - `Borrowed_Books`: Records of borrowed books.

- **People Related Tables**:
  - `member`: Information about library members.
  - `employee`: Details of library employees.
  - `Position`: Employee positions within the library.

- **Place Related Tables**:
  - `branch`: Details of library branches.
  - `city`: Information about cities where branches are located.
  - `province`: Data related to provinces.
  - `country`: Information about countries.

- **Cultural Tables**:
  - `research`: Records of research activities.
  - `event`: Details of library events.

- **Financial Tables**:
  - `budget`: Information about library budgets.
  - `salary`: Salary details of employees.
  - `buyheader`: Records of purchases made.

## datawarehouse

### Data Marts

Our datawarehouse consists of three data marts:

1. **Financial Data Mart**:
   - `transactional fact`: Records of financial transactions.
   - `monthly periodic snapshot fact`: Snapshot data on a monthly basis.
   - `accumulative fact`: Accumulated financial data.
   - `salary transactional fact`: Records of salary transactions.

2. **Cultural Data Mart**:
   - `research transactional fact`: Records of research activities.
   - `research monthly periodic snapshot fact`: Monthly snapshots of research data.
   - `event transactional fact`: Records of library events.

3. **Lending Data Mart**:
   - `Transactional fact`: Records of lending transactions.
   - `daily periodic snapshot fact`: Snapshot data on a daily basis.
   - `accumulative fact`: Accumulated lending data.

## ETL (Extract, Transform, Load)

We have implemented ETL processes to populate the datawarehouse:

- **Loading Datawarehouse**: Processes for loading data into the datawarehouse.
- **Dimensions First and Incremental Load**: Strategies for loading dimension tables.
- **Facts First and Incremental Load**: Strategies for loading fact tables.

## ETL Jobs

We have included ETL jobs to automate the data extraction, transformation, and loading processes

## Project Contributors

This project was a collaborative effort involving three dedicated individuals:

- [Marzia Nouri](https://github.com/marzinouri)
- [Elaheh Toulabinejad](https://github.com/ellietoulabi/)
- [Mohammad Mirsafaei](https://github.com/MohammadMirsafaei)

We all contributed to the design, development, and maintenance of this library datawarehouse project.
